# Strike Fitness Technical Architecture

**Status:** Architecture decision for initial implementation  
**Project stage:** Strategy and design complete; application implementation not started  
**Document date:** October 2026  
**Source documents:** Business and brand brief, landing-page strategy, landing-page wireframe, refined creative direction, and visual design system

## 1. Purpose

This document defines the technical direction for the Strike Fitness pre-launch marketing site and the boundary through which it can later participate in an end-to-end marketing technology workflow:

> Visitor → Landing Page → Lead Capture → ESP/CRM → Lead Properties → Segmentation → Lifecycle Messaging → Engagement → Analytics

The architecture is intended to keep the first implementation simple, understandable, and faithful to the approved strategy and design. It establishes boundaries and decision criteria rather than prescribing implementation steps.

The governing principles are:

- Keep the frontend simple and avoid unnecessary frameworks.
- Build only what the current single-page experience requires.
- Keep presentation, lead transport, and Martech responsibilities separate.
- Do not expose ESP/CRM credentials or privileged operations in the browser.
- Preserve a stable lead-capture boundary so a future vendor can be integrated without rebuilding the page.
- Prefer explicit, accessible browser behavior over application-style abstraction.
- Add infrastructure only when a demonstrated requirement justifies it.
- Keep the project legible to another developer reviewing the portfolio.

## 2. Current Scope

The repository currently contains research, strategy, and design documentation only. It has no application source, package manifest, build configuration, tests, or deployed integration. The README also identifies application and Martech implementation as later phases.

The initial product is one mobile-first marketing page at `/`. Its purpose is to explain the proposed Strike concept, establish trust about its pre-launch status, and collect qualified, permissioned interest. It is not a membership application, customer account, scheduling system, or general fitness website.

Current scope includes:

- One responsive, accessible landing page.
- On-page anchor navigation and one consistent primary CTA path.
- One canonical lead form.
- Client-side field interaction, validation, loading, error, and inline success states.
- A replaceable boundary for future lead submission.
- Architectural seams for future website analytics.

Current scope does not include a separate thank-you page, additional marketing pages, a customer database, authentication, membership features, or an implemented ESP/CRM workflow.

## 3. Technology Stack

### Vite

Vite is the development server and production build tool. It provides a fast local workflow, TypeScript module support, asset handling, and an optimized static production build without imposing a frontend application framework.

### TypeScript

TypeScript provides explicit contracts for form values, controlled interest values, lead-submission outcomes, UI states, and analytics events. Its role is to make boundaries understandable and reduce accidental coupling; it should not be used to recreate a framework or introduce class-heavy architecture.

### Tailwind CSS

Tailwind CSS is the styling layer. The approved design-system roles—color, typography, spacing, breakpoints, radii, focus, and interaction states—should be represented through a small semantic project theme and consistent component patterns. Raw utility use should remain subordinate to the design system rather than creating an unrelated visual vocabulary.

### npm

npm is the package manager and script runner. Dependencies should remain few, current, and tied to a demonstrated requirement. A dependency should not be added when browser APIs or a small project-owned module can solve the problem clearly.

### Browser/client-side JavaScript

Browser JavaScript progressively enhances semantic HTML. It owns on-page navigation behavior, the optional second-interest interaction, accessible FAQ disclosure, form validation feedback, submission state, inline confirmation, and website-originated event dispatch.

The browser must not own secret credentials, authoritative consent or signup timestamps, lead deduplication, lifecycle-stage changes, or direct privileged administration of an ESP/CRM.

## 4. Frontend Architecture

The site should use semantic HTML as the document structure, Tailwind for styling, and small TypeScript modules for behavior. Vanilla TypeScript is sufficient because the page has one route, limited shared state, and a narrow set of interactions.

The frontend should be organized by responsibility rather than by visual fragment:

- **Page composition:** Semantic sections, headings, landmarks, status labels, and the canonical form.
- **UI behavior:** Anchor focus handling, FAQ disclosure, optional-interest reveal/removal, and any validated mobile CTA behavior.
- **Lead capture:** Form state, validation, payload construction, submission coordination, and result handling.
- **Lead gateway:** One transport-facing contract that accepts a lead payload and returns a small, vendor-neutral result.
- **Analytics boundary:** One website event dispatcher with no vendor-specific calls in presentation modules.
- **Configuration and controlled values:** Stable interest identifiers, form identifiers, page variant, and approved environment-dependent public configuration.

Presentation modules should call the lead gateway and analytics boundary; they should not know whether a future integration uses Klaviyo, HubSpot, a serverless function, or another service. Likewise, analytics code should observe meaningful outcomes rather than control the form.

There is no need for a client-side router, global state library, component runtime, or generalized design-system package. Shared UI patterns may be expressed through semantic markup, Tailwind composition, and focused TypeScript behavior. The architecture should preserve native browser semantics wherever possible.

Accessibility is an architectural requirement, not a finishing pass. The implementation should target WCAG 2.2 Level AA, preserve logical document and focus order, expose validation and submission status to assistive technology, respect reduced motion, and keep the page usable without framework-specific rendering behavior.

## 5. Initial Site Structure

The Home page at `/` should implement the approved problem-to-action journey. The existing landing-page strategy, wireframe, creative direction, and design system remain the source of truth for content order, copy development, visual treatment, responsive behavior, and interaction states.

The major conceptual sections are:

1. Development-status notice.
2. Minimal header with optional “How it works” and FAQ anchors plus the primary CTA.
3. Hero and primary value exchange.
4. The gap between access without direction and guidance without flexibility.
5. The proposed connected experience: independent training, a clear path, coached sessions, and optional personal support.
6. Key experience benefits: a clear next step, real-life fit, useful training space, and support without pressure.
7. Audience relevance and fitness interests.
8. Trust, current development status, and the progression from unknowns to real proof.
9. What subscribers can expect.
10. The canonical lead form and interest selection.
11. Focused FAQ and objection handling.
12. Final CTA linking back to the same form.
13. Minimal footer.

All primary CTA placements lead to the same form and preserve any entered state. The initial page should not contain duplicate independent forms, full-site navigation, speculative pages, or competing booking, purchase, social, and download conversions.

The design should follow the approved Grounded Momentum system: clear hierarchy, warm structure, measured progression, one restrained action accent, accessible states, and honest distinction between confirmed facts, intended principles, proposed features, and unknowns.

## 6. Lead Capture Architecture

The lead-capture boundary is:

> Landing-page form → validated lead payload → lead gateway → future integration boundary → ESP/CRM result → inline page state

### Browser responsibilities

The browser should:

- Collect only the approved visible fields.
- Validate required values and controlled interest choices.
- Preserve valid input after validation or integration failure.
- Capture non-sensitive page and acquisition context available to the site.
- Prevent accidental duplicate submission while a request is in progress.
- Send the payload through one lead gateway.
- Display success only after the integration reports that the record was accepted or reliably queued.
- Display a clear retryable failure state without claiming that a lead exists.

The initial visible form contains `first_name`, `email`, required `primary_interest`, and optional `secondary_interest`. The interest fields use stable internal values even if visitor-facing labels later change.

The broader conceptual profile may also contain `last_name`, `lead_source`, and `signup_date`, but these do not all belong in the first browser payload:

- `last_name` remains absent and unset at first touch. The approved landing-page strategy explicitly removes it from the initial form; it may be collected later only for a concrete operational need.
- `lead_source` is derived from approved acquisition context rather than entered by the visitor.
- `signup_date` is assigned by the receiving system using an authoritative timestamp rather than trusted from the browser.

Consent status, consent timestamp, disclosure version, and source context are required operational metadata around the profile, not reasons to expand the visible form.

### Future integration responsibilities

The eventual server-side or vendor-supported integration should:

- Validate and normalize the payload again.
- Apply authoritative timestamps and consent context.
- Create or update a profile using email as the initial identifier.
- Deduplicate repeat submissions.
- Map stable site values to vendor properties.
- Protect credentials and enforce abuse controls.
- Return a vendor-neutral result such as created, updated, accepted for processing, or failed.
- Emit or make available the authoritative lead outcome for analytics reconciliation.

The production site should not call privileged ESP/CRM APIs directly from browser code. No backend should be built until the selected vendor and its secure integration options establish what boundary is actually needed. Until then, the frontend contract can be defined and tested without presenting a simulated submission as a real conversion.

Successful submission remains on `/` and replaces or updates the form region with a calm inline success state. The state should confirm the communication expectation, acknowledge the selected interest without overpersonalizing, and make clear that signup is not membership enrollment.

## 7. Martech Architecture

The future Martech layer should remain conceptually separate from the page:

1. The landing page collects a minimal, permissioned profile and acquisition context.
2. The integration creates or updates the ESP/CRM profile.
3. Stable properties support simple, action-oriented segments.
4. Segments influence message emphasis, timing, or invitations.
5. Lifecycle flows send useful communications tied to the visitor's stage.
6. Engagement data informs later segmentation and funnel analysis without silently replacing stated preferences.

The minimal marketing-relevant profile is:

- `first_name`
- `last_name` — unset initially and deferred until needed
- `email`
- `primary_interest`
- `secondary_interest` — nullable
- `lead_source`
- `signup_date`

Interest values should use a controlled taxonomy aligned with the approved five visitor-facing choices. Primary interest is the main initial relevance signal; secondary interest refines it. Neither should be treated as a complete identity, ability level, health status, or purchase intent.

Initial segmentation should remain limited to dimensions that change communication or analysis, principally stated interest, lifecycle stage, and normalized acquisition source. Lifecycle messaging may later include welcome, pre-launch progress, interest-relevant education, and real event, preview, tour, or enrollment transitions. These are conceptual programs, not current automations.

The ESP/CRM should be the system of record for contact permission and lifecycle messaging once selected. General analytics should not receive names, email addresses, or other direct identifiers.

## 8. Analytics Architecture

Project analytics events use lower-case `snake_case` and past-tense action names. Each name describes something that has already occurred, not an interface label or future intent. Future events must follow the same convention, have one documented firing rule and owner, and carry context in properties rather than multiplying names by placement or page variant.

### Website-originated events

The website can originate behavior it directly observes:

- `landing_page_viewed`
- `primary_cta_clicked`
- `lead_form_started`
- `fitness_interest_selected`
- `lead_form_validation_failed`
- `lead_form_submitted`
- `signup_confirmed`

These names retain the more precise taxonomy already established in the landing-page strategy. Broader concepts such as `cta_clicked`, `form_started`, `interest_selected`, and `form_completed` should not be emitted as duplicate aliases. If a broader naming system is adopted later, names should be migrated deliberately rather than double-fired.

`lead_form_submitted` records that a valid payload left the browser. It is not the primary conversion because processing may still fail. The term `form_completed` is therefore avoided: it can incorrectly imply both browser completion and successful record creation.

### Integration-originated events

The secure integration or lead system owns authoritative record outcomes:

- `lead_created`
- `lead_updated`
- `lead_creation_failed`

`lead_form_submitted` and `lead_created` are related but not redundant. The first measures visitor intent and transport initiation; the second confirms the business outcome. Their difference exposes integration loss. A non-PII conversion identifier may reconcile the two.

`signup_confirmed` is a website UX event shown only after an accepted lead outcome. It is useful for diagnosing whether technical success was communicated, but it should not replace `lead_created` or `lead_updated` in conversion reporting.

### ESP/CRM and lifecycle events

The ESP/CRM or messaging layer owns delivery and engagement events:

- `email_sent`
- `email_opened`
- `email_clicked`

These must not be synthesized by the website. `email_sent` reflects provider acceptance or send status according to a documented definition. `email_opened` is directionally useful but technically noisy because privacy protection and image loading can create false or missing opens; it should not be treated as definitive engagement. `email_clicked` is generally a stronger engagement signal, subject to bot and security-scanner filtering.

If a selected analytics platform already records a generic page view automatically, the project should choose either that event or `landing_page_viewed` as the canonical denominator rather than counting both. Analytics implementation, vendor selection, consent treatment, attribution rules, and event transport are deferred.

## 9. Deferred Decisions

The following are intentionally not decided or implemented now:

- Klaviyo versus HubSpot.
- The exact backend, API, serverless, or vendor-native integration architecture.
- A first-party database.
- Authentication or customer accounts.
- Additional pages such as Classes, Personal Training, About, or Contact.
- React or another client-side framework.
- Astro or another content/site framework.
- Advanced analytics infrastructure, tag management, identity resolution, or attribution modeling.
- Final analytics vendor and consent-management approach.
- Lifecycle automation details, send cadence, and email content.
- A separate `/thank-you` page.
- Final deployment and hosting provider.

These are deferred because current requirements do not establish a need or because a later vendor, operational, legal, content, or measurement decision must come first.

## 10. Evolution Path

Architectural complexity should increase only when observed requirements exceed the current design:

- **More pages:** Introduce shared page composition or reconsider the site architecture when real, maintained content requires multiple routes and duplicated structure becomes costly. Additional pages alone do not automatically require a framework.
- **Richer client state:** Consider React or another stateful UI approach only when the site develops sustained, interdependent state that is materially difficult to manage with focused TypeScript—for example, multi-step enrollment, authenticated account tools, or complex live scheduling.
- **Content-driven build needs:** Reconsider Astro only if a larger set of content pages, templates, content collections, or publishing workflows makes static page composition difficult to maintain.
- **Server-side needs:** Add a backend boundary when secure credential handling, provider restrictions, abuse prevention, webhooks, authoritative validation, cross-system orchestration, or reliable retry behavior requires it.
- **Data persistence:** Add a database only if the ESP/CRM and integration logs cannot meet a defined operational or reporting requirement.
- **Martech integration:** Implement the smallest secure adapter supported by the selected ESP/CRM. Keep vendor mapping beyond the frontend lead contract.
- **Analytics maturity:** Add dedicated tooling when specific questions require cross-channel reconciliation, governance, consent controls, or reporting that the site and ESP/CRM cannot provide simply.
- **Thank-you route:** Consider a dedicated post-submission page only when conversion tracking, campaign destination needs, shareability, or a meaningful next-step journey cannot be handled reliably by the inline state.
- **Testing depth:** Expand automated coverage in proportion to behavioral risk, especially around lead payload validation, gateway outcomes, accessible form states, and event firing rules.

The default remains the smallest architecture that accurately supports the current page, protects visitor trust, and leaves clear seams for demonstrated future needs.
