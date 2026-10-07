# Strike Fitness Landing-Page Wireframe

**Status:** Low-fidelity content and conversion architecture  
**Company:** Strike Fitness  
**Page stage:** Concept validation and pre-launch  
**Primary source of truth:** `docs/strategy/strike-business-brand-brief.md`  
**Supporting strategy:** `docs/strategy/strike-landing-page-strategy.md`  
**Competitive inputs:** `docs/research/crunch-company-research.md` and `docs/research/crunch-local-opening.md`

## Purpose of This Document

This document defines the structure, information order, conversion path, and content responsibilities of the first Strike Fitness landing page. It is detailed enough to guide low-fidelity design and implementation planning, but it is not final copy, a visual design, or production code.

The page has one primary conversion objective:

> A relevant visitor submits their first name, email address, and one primary fitness interest to receive appropriate Strike Fitness launch updates and opportunities.

An optional second interest may be added after the required primary interest is chosen.

The page is not trying to sell a membership yet. Strike has no operating location, final site, confirmed opening date, final pricing, completed facility, or verified member outcomes. The architecture must make the proposed experience understandable and worth following without presenting planning assumptions as facts.

## 1. Overall Page Hierarchy

### Recommended page sequence

1. Development-status notice
2. Header and minimal navigation
3. Hero and primary value exchange
4. The gap Strike is designed to fill
5. The proposed Strike experience
6. Key experience benefits
7. Audience relevance and fitness interests
8. Trust, current status, and proof
9. What subscribers can expect
10. Lead capture and fitness-interest selection
11. Focused FAQ and objection handling
12. Final CTA
13. Minimal footer

### Why this order

The sequence follows the decisions a visitor needs to make:

1. **Orient:** What is Strike, and is it open?
2. **Recognize:** Does it understand why my current routine is difficult to sustain?
3. **Differentiate:** Is this meaningfully different from an access-only gym or fixed-format studio?
4. **Evaluate fit:** Would the intended experience work for the way I want to train?
5. **Trust:** Is Strike being candid about what exists and what remains unknown?
6. **Understand the exchange:** What will I receive if I share my information?
7. **Act:** Can I sign up quickly without making a membership commitment?

The form appears once as the main conversion module near the end of the explanatory journey. Earlier and later primary CTAs lead to that same form. They do not open competing flows.

### Page-level conversion rules

- Use one primary action concept throughout: join the Strike interest list for relevant launch updates and opportunities.
- Make every primary CTA point to the same lead form.
- Use an on-page learn-more link only as a subordinate micro-conversion.
- Do not introduce booking, purchasing, membership enrollment, social following, content downloads, or partner inquiries as competing conversions.
- Do not use fake urgency, countdowns, founder-rate language, speculative discounts, or unsupported scarcity.
- Do not imply that joining the list makes someone a member or guarantees priority access.
- Keep the development stage visible, but do not let caveats replace the customer benefit.
- Use ordinary, grounded language. Avoid aggression, combat metaphors, body shame, transformation promises, and generic category superlatives.

### High-level low-fidelity map

```text
[Development status]

[Logo]                         [How it works] [FAQ] [Primary CTA]

[Hero: problem + proposed answer + pre-launch value exchange]
[Primary CTA] [Subordinate learn-more link]

[The gap: access without direction vs. guidance without flexibility]

[Proposed experience: open gym + training paths + coached sessions + optional support]

[Key benefits: clear next step | usable space | flexible support | respectful experience]

[Audience relevance: needs and fitness interests]

[Trust: what is known | what is still in development | real proof when available]

[Subscriber value: what updates may include and what signup does not mean]

[Lead form]
  First name
  Email
  Primary fitness interest
  Optional second interest
  Permission/privacy context
  Primary CTA

[Focused FAQ]

[Final CTA linking back to the same form]

[Minimal footer]
```

## 2. Header and Navigation

### Purpose

Identify Strike, provide only the orientation paths needed to understand the concept, and keep the primary action visible without creating unnecessary exits.

### Main message

Strike Fitness is a new fitness concept in development, and the next meaningful action is to receive relevant updates.

### Important content

- Strike Fitness wordmark or text logo.
- Two optional anchor links:
  - **How it works** — moves to the proposed experience.
  - **Common questions** — moves to the FAQ.
- One primary CTA that moves to the lead form.
- A short development-status line above or within the header if the hero does not make the stage immediately unmistakable.

The header should become simpler on mobile. A menu is unnecessary if only two anchor links exist; those links may be omitted from the smallest viewport while retaining the logo and primary CTA.

### CTA

Use the same benefit-led primary CTA concept used everywhere else on the page. The final label should accurately communicate joining an interest or update list, not joining the gym.

### Conversion goal

Give high-intent visitors a direct route to the form while keeping less-ready visitors on the page long enough to understand the concept.

### What should NOT be included

- Full site navigation for pages that do not yet exist.
- Membership, pricing, schedule, location, amenities, or class links before those details are confirmed.
- Social-media icons competing with the primary CTA.
- “Join now,” “Become a member,” or other enrollment language.
- Phone numbers or sales-chat prompts without a staffed, defined support process.
- A large mobile menu for a single-purpose page.

## 3. Hero Section

### Purpose

Explain the customer problem, Strike's intended answer, and the reason to engage before launch within the first screen.

### Main message

Strike is being built to make fitness consistency easier by combining the freedom of a gym with clear, flexible guidance.

The hero should communicate three ideas in this order:

1. The visitor does not necessarily need more motivation or more access; they may need a more usable way to train consistently.
2. Strike intends to connect independent training, clear training paths, coached sessions, and optional support.
3. Strike is still in development, and visitors can receive relevant updates as real details and opportunities become available.

This is message direction, not final headline copy.

### Important content

- A concise, problem-led headline.
- One short supporting statement explaining the freedom-plus-guidance proposition.
- A visible pre-launch or “in development” label.
- A brief value-exchange statement explaining why signup is useful now.
- Primary CTA to the form.
- Optional subordinate anchor link to the proposed experience.
- If imagery is used later, it should communicate ordinary adults training with clarity and confidence without implying it depicts an operating Strike club.

### CTA

- **Primary:** Scroll to the lead form.
- **Secondary:** An understated text link such as learning how the concept is intended to work; it remains on-page.

### Conversion goal

Create enough relevance and understanding that a high-intent visitor is willing to begin signup, while giving cautious visitors a clear reason to continue.

### What should NOT be included

- Unverified city, address, opening date, price, membership offer, or facility specification.
- Finished-facility renderings presented as fact.
- An exhaustive service or amenity list.
- Multiple equal-weight CTAs.
- Generic claims such as “something for everyone,” “world-class,” “state-of-the-art,” or “unbeatable value.”
- Appearance-led transformation language or before-and-after imagery.
- High-intensity or combative uses of the Strike name.

## 4. Primary CTA System

### Purpose

Make one action recognizable throughout the page and prevent visitors from having to interpret different labels as different commitments.

### Main message

Share minimal information to receive relevant Strike launch updates and real opportunities as they become available.

### Important content

- Use one consistent CTA concept in:
  - Header.
  - Hero.
  - One contextual point after the experience or subscriber-value explanation, if needed.
  - Form submission.
  - Final CTA.
- Anchor CTAs should scroll to the same form and preserve any information already entered.
- The submission CTA may be more explicit than the anchor CTA, but both must describe the same commitment.
- A restrained mobile sticky CTA may be tested if it links to the form, does not obscure content, and disappears when the form is in view.

### CTA

The exact label requires copy development and comprehension testing. It should communicate receiving updates or expressing interest. It must not use a generic “Submit” label or imply membership enrollment.

### Conversion goal

Reduce decision friction and increase qualified form starts without increasing the apparent commitment.

### What should NOT be included

- Different primary actions in different sections.
- “Join Strike,” “Buy now,” “Reserve membership,” or “Claim your spot” before a real offer exists.
- Countdown timers or “last chance” treatment.
- Pop-ups that interrupt reading or unexpectedly replace the page.
- Repeated CTA blocks after every section.
- A sticky CTA that competes with the form or privacy disclosure.

## 5. Value Proposition: The Gap Strike Is Designed to Fill

### Purpose

Make the category difference legible before describing features. Visitors should understand why Strike is not simply another gym with more marketing language.

### Main message

Many gyms provide access but little direction. Many studios provide direction but require a narrow format, fixed schedule, or higher level of commitment. Strike is intended to occupy the practical middle: guidance without boutique rigidity.

### Important content

- A concise comparison based on customer trade-offs:
  - **Access-only experience:** freedom, but the visitor may still wonder what to do or how to progress.
  - **Fixed-format experience:** coaching and energy, but less control over schedule or training style.
  - **Strike's intended middle:** independent training, clear paths, and flexible support connected in one experience.
- The customer problem remains consistency, not the inferiority of a named competitor.
- A short bridge explaining the practical benefit: knowing the next step while retaining choices when schedules and needs change.

This can be represented as a simple three-part content structure. It should not become a feature-comparison chart with unsupported checkmarks.

### CTA

No standalone primary CTA is required inside the comparison. An optional text link may move to the proposed experience immediately below.

### Conversion goal

Increase proposition comprehension so that visitors see value in following Strike even before price, site, or opening timing is available.

### What should NOT be included

- Named attacks on Crunch or any other competitor.
- Claims that Strike is cheaper, better, less crowded, cleaner, or more effective without evidence.
- Competitor logos, prices, slogans, or proprietary program names.
- A universal claim that every gym is impersonal or every studio is inflexible.
- A dense matrix of speculative features.

## 6. Fitness Experience and Offering

### Purpose

Show how the intended experience works as a connected system. This section answers “What would I actually be able to do?” without publishing an unconfirmed facility, class schedule, or membership catalog.

### Main message

Strike is intended to let people choose the amount of structure they need while maintaining a clear path forward.

### Important content

Use four sequential experience components:

1. **Train independently**
   - Open-gym freedom for strength, cardio, and movement work.
   - Guidance is available but not forced.
2. **Follow a clear path**
   - Simple, coach-designed starting points and progression.
   - The benefit is less decision fatigue, not a promise of a specific proprietary program.
3. **Use coached sessions**
   - Focused group guidance can provide technique, structure, and accountability.
   - Formats and schedules remain subject to validation.
4. **Add personal support when useful**
   - Optional one-to-one or small-group guidance for more help.
   - It should not appear mandatory or become a personal-training sales pitch.

The section should show how a visitor can move between these levels as life, confidence, or goals change. The model is one connected experience, not four unrelated products.

### CTA

An optional, subordinate transition can invite the visitor to identify the kind of fitness they care about, leading into audience relevance and interest selection. It should not ask for data yet.

### Conversion goal

Resolve concept ambiguity and help both independent exercisers and guidance-seeking visitors see a plausible fit.

### What should NOT be included

- Final membership tier names or inclusions.
- Final class names, timetable, session limits, or booking policies.
- Exact square footage, equipment counts, branded zones, or amenity commitments.
- A long list of speculative offerings.
- Claims of individualized programming for every person.
- Medical, rehabilitation, injury-treatment, or guaranteed-outcome language.
- An implication that personal training is required.

## 7. Key Benefits

### Purpose

Translate the proposed operating model into a small number of customer-relevant reasons to care.

### Main message

The intended value of Strike is a more usable and respectful fitness experience: a clear next step, room to do the work, and support that can adapt.

### Important content

Use no more than four benefit themes:

1. **A clear next step**
   - Reduce uncertainty about how to begin and what to do next.
2. **Training that can fit real life**
   - Combine independent access and scheduled guidance instead of requiring one fixed mode.
3. **Space designed for useful training**
   - Prioritize practical training zones and capacity awareness over a long amenity list.
4. **Support without pressure**
   - Make guidance, communication, future pricing, and terms straightforward and respectful.

Until operations exist, these must be framed as design principles or intended standards—not proven outcomes.

### CTA

No dedicated CTA is necessary. If a mid-page primary CTA is used, place it after this section and send it to the same form.

### Conversion goal

Convert an abstract hybrid concept into memorable practical value, preparing the visitor to evaluate personal relevance.

### What should NOT be included

- More than four or five benefit claims.
- Unsupported promises about cleanliness, equipment availability, coaching quality, retention, or results.
- “Best,” “premium,” “elite,” “revolutionary,” or similar unsubstantiated language.
- Amenities included only because competing gym pages list them.
- Benefits based solely on appearance, weight loss, or intensity.

## 8. Audience Relevance

### Purpose

Help visitors recognize themselves by need and training preference without fragmenting the page into demographic personas.

### Main message

Strike is being designed for adults who want fitness to become a realistic, repeatable part of life—whether they prefer training independently, value group energy, want more guidance, or are returning after a lapse.

### Important content

Use a concise set of need-based recognition statements:

- “I want to build or maintain strength without guessing what to do.”
- “I want cardio or conditioning options that fit my routine.”
- “I like group guidance, but I also need schedule flexibility.”
- “I want to move better and balance higher-effort training.”
- “I want a clear, low-pressure way to begin or restart.”

These statements should map conceptually to the five fitness-interest choices without forcing visitors to classify themselves by ability, age, body type, or identity.

The section should state that experienced independent exercisers remain a real audience: guidance is available, not compulsory.

### CTA

A light transition may invite the visitor to choose the interest most relevant to them when they reach the form. Do not present a separate quiz.

### Conversion goal

Increase self-recognition, reduce intimidation, and make the later interest selection fast and understandable.

### What should NOT be included

- Separate pages or tabs for each persona.
- Narrow demographic targeting based on unvalidated age, income, gender, household type, or life stage.
- “Everyone is welcome” as a substitute for operationally credible relevance.
- Labels such as beginner, unfit, inactive, overweight, or advanced as required classifications.
- Medical conditions, injury status, or recovery claims.
- A goal quiz that adds another funnel.

## 9. Trust, Development Status, and Social Proof

### Purpose

Build credibility through specificity and honesty. Strike has no legitimate member proof yet, so the section must explain the current stage and distinguish proposals from confirmed facts.

### Main message

Strike is new and in development. Confirmed location, timing, pricing, and opportunities will be shared when they are real.

### Important content

Use a compact “What is known / What is still being developed” structure.

**What is known**

- Strike is a new independent fitness concept.
- It is being designed around flexible guidance, practical training, and respectful service.
- The page is collecting permissioned interest and learning which fitness experiences matter to prospects.

**What is still being developed**

- Location and local trade area.
- Opening timing.
- Facility and equipment decisions.
- Programming and schedule.
- Memberships, pricing, and policies.

**Proof progression**

As real evidence becomes available, this section may add:

- Founder identity, rationale, and relevant experience.
- Confirmed site and local context.
- Real build progress.
- Confirmed equipment or space decisions.
- Identified coaches with accurate credentials.
- Actual pop-ups, previews, or substantive local partnerships.
- Published membership terms and policies.

Each proof item must be dated or contextualized where recency matters. The page should remove generic placeholder language when specific proof becomes available.

### CTA

No independent CTA is needed. The section should naturally support the later signup by making updates feel useful and credible.

### Conversion goal

Reduce skepticism caused by pre-launch uncertainty without manufacturing social proof.

### What should NOT be included

- Testimonials, reviews, ratings, member counts, outcome statistics, or partner logos that do not yet exist.
- Stock photos presented as Strike members, staff, classes, or facilities.
- Crunch's company scale, class-attendance data, opening tactics, or facility facts as proof for Strike.
- Generic “trusted by” modules.
- Renderings without clear labeling.
- Implied local roots before a local market or site is established.
- Vague claims of “overwhelming demand.”

## 10. What Subscribers Can Expect

### Purpose

Make the value exchange and communication permission explicit before asking for personal information.

### Main message

Subscribers can receive useful, relevant updates as Strike's plans become real; signup is not a membership commitment.

### Important content

Describe only communication categories Strike is prepared to deliver:

- Meaningful development and opening updates.
- Notice when real tours, previews, pop-ups, or memberships become available.
- Information connected to the subscriber's chosen fitness interest.
- Appropriate invitations to provide input on pre-launch decisions.

Also state:

- Not every category is guaranteed immediately.
- Signup does not create a membership or payment obligation.
- Strike will not use the form as permission for unrelated contact.
- Visitors can unsubscribe.

The exact expectation should be revised at launch to reflect the communications Strike can actually support.

### CTA

A single primary CTA may appear after this explanation and move to the form directly below.

### Conversion goal

Improve permission quality by ensuring visitors understand the benefit and scope of communication before submitting.

### What should NOT be included

- “Join our newsletter” as the only value proposition.
- A guaranteed cadence that has not been operationally planned.
- Guaranteed early access, discounts, founder status, or priority placement.
- Promised events, previews, or memberships that do not yet exist.
- Content downloads added only to create a lead magnet.
- SMS or phone promises when the page does not collect channel-specific permission.

## 11. Lead Capture Section

### Purpose

Collect the minimum information required to create a useful, permissioned lead and provide relevant future communication.

### Main message

Tell Strike how to contact you and what fitness topic matters most so future updates can be more relevant.

### Important content

The visible form contains:

1. **First name — required**
   - Use the person's preferred first name.
2. **Email address — required**
   - This is the communication channel and initial profile identifier.
3. **Primary fitness interest — required**
   - One selection from the defined five-option taxonomy.
4. **Secondary fitness interest — optional**
   - Offered only after the primary choice.
   - Uses the same taxonomy, excluding the selected primary option.
   - Maximum of two total interests.

Form behavior:

- Present the interest options as large, easily scanned controls.
- Do not preselect an interest.
- Keep helper descriptions short.
- State clearly that the second interest is optional.
- Use inline validation and preserve all valid entries after an error.
- Put concise permission and privacy context immediately beside the submission action.
- Link to the privacy notice.
- Confirm success only after the lead system accepts or updates the record.
- In the confirmation state, restate expected communications, acknowledge the selected primary interest, and clarify that signup is not a membership commitment.

### CTA

The submission label should describe receiving relevant updates or recording interest. It should not say only “Submit,” and it should not imply membership.

### Conversion goal

Create or update a valid lead record with contact information, stated interest, source context, timestamp, and consent context while minimizing friction.

### What should NOT be included

- Last name.
- Phone number or SMS consent.
- Address, ZIP code, or neighborhood before a location-dependent use exists.
- Age, date of birth, gender, income, occupation, employer, or household details.
- Weight, body measurements, appearance goals, photos, diagnoses, medications, injuries, or medical history.
- Current gym, budget, purchase readiness, preferred workout time, or experience level.
- Open-ended goal text.
- Account credentials.
- A required consent checkbox added by habit if the signup action and disclosure already create valid, explicit permission; legal requirements must govern the final treatment.

## 12. Fitness-Interest Selection

### Purpose

Create immediate relevance for the visitor, useful demand signals for Strike, and a defensible basis for later message personalization.

### Main message

Choose the area you care about most, with an optional second choice if two areas matter.

### Important content

Use these five consumer-facing options:

1. **Strength training**
   - Free weights, weight machines, and functional strength workouts.
2. **Cardio workouts**
   - Treadmills, stair climbers, bikes, and other cardio training.
3. **Group fitness classes**
   - Instructor-led strength, cardio, and movement classes.
4. **Yoga & Pilates**
   - Yoga, Pilates, stretching, and mobility-focused sessions.
5. **Personal training & guidance**
   - Individual or small-group help with getting started, making progress, or staying consistent.

Interaction requirements:

- The primary choice is required and visibly identified as primary.
- After selection, reveal an “Add a second interest — optional” action.
- The second control uses the same five categories but removes the primary selection.
- The interface must never allow more than two total selections.
- Visitors must be able to change or remove the optional choice.
- On mobile, labels and helper text must remain readable without opening five separate explanatory dialogs.
- The options describe areas of interest, not confirmed Strike programs or amenities.

Before publishing, verify that every helper example remains genuinely under consideration. If a named format or equipment type is no longer part of the concept, revise the helper text.

### CTA

Interest selection is part of the lead form, not a separate conversion. No CTA is needed beyond proceeding to form submission.

### Conversion goal

Capture one useful declared preference without making the visitor complete a research survey or disclose sensitive goals.

### What should NOT be included

- More than five primary choices in the first version.
- An “Other” option that requires free-text entry.
- Preselected or inferred interests.
- Weight loss, body transformation, injury recovery, medical improvement, or diagnosis-related choices.
- Internal terminology such as “conditioning” or “mobility” without familiar consumer framing.
- “Beginner” or “advanced” as fitness-interest categories.
- Separate interest-specific landing-page narratives at this stage.

## 13. Focused FAQ and Objection Handling

### Purpose

Resolve the small number of uncertainties most likely to prevent signup after the concept and value exchange are understood.

### Main message

Strike will answer what it can, name what remains unknown, and explain how subscribers will receive confirmed information.

### Important content

Limit the initial FAQ to questions that materially affect the lead decision:

1. **Is Strike open yet?**
   - No; it is in development.
2. **Where will it be located?**
   - No site is confirmed; do not imply a city or trade area.
3. **When will it open?**
   - No date is confirmed; meaningful timing updates are part of the signup value.
4. **What will membership cost?**
   - Pricing is not final; Strike intends to publish clear total pricing and terms when validated.
5. **Does signing up make me a member?**
   - No; it records interest and communication permission only.
6. **What happens after I sign up?**
   - A genuine confirmation followed by relevant updates as useful information becomes available.
7. **How will my information be used?**
   - To deliver the requested updates and make them more relevant based on selected interests, subject to the privacy notice and unsubscribe controls.
8. **Will I be pressured to buy personal training?**
   - The intended model treats guidance as optional and sales as respectful; avoid making an operational guarantee beyond what Strike has established.

Answers should be direct and short. Unknowns are valid answers.

### CTA

After the final FAQ answer, present the final CTA linking to the same form.

### Conversion goal

Remove uncertainty that is preventing an otherwise relevant visitor from completing the form.

### What should NOT be included

- A comprehensive support center.
- Questions visitors are unlikely to ask at this stage.
- Invented answers about parking, hours, equipment, childcare, showers, contracts, guest access, or class schedules.
- Reassurance claims that operations cannot yet prove.
- Competitor comparisons.
- Legal text that belongs in the privacy notice or terms.

## 14. Final CTA

### Purpose

Give visitors who needed the full explanation a clear, low-commitment next step without introducing a new offer.

### Main message

If the Strike concept fits what the visitor is looking for, they can receive relevant updates as confirmed details and real opportunities become available.

### Important content

- A short restatement of the core value exchange.
- A reminder that Strike is in development.
- The same primary CTA concept used in the header and hero.
- The CTA scrolls to the existing form and retains any information already entered.
- If the form sits immediately above the FAQ, this module can be compact; it should not repeat the entire hero.

### CTA

Link to the lead form. Do not create a second independent form unless testing demonstrates a clear mobile usability need and both instances share state and validation.

### Conversion goal

Convert informed visitors after their concept, fit, trust, and privacy questions have been addressed.

### What should NOT be included

- A new discount, offer, deadline, event, or membership proposition.
- Social follow buttons as an alternative conversion.
- “Act now” pressure.
- A second set of fields that can produce conflicting data or duplicate submissions.
- New claims that did not appear earlier on the page.

## 15. Footer

### Purpose

Provide company identification, privacy access, and communication reassurance without opening unnecessary exit paths.

### Main message

Strike is a new independent fitness concept that will handle visitor information and communication transparently.

### Important content

- Strike Fitness company identification.
- Current year.
- Privacy notice link.
- Contact method only if an inbox or process is actively monitored.
- Concise unsubscribe or communication-control reassurance.
- Any legally required links or disclosures.

### CTA

No conversion CTA is required. If included, it must remain visually subordinate to the page's completed conversion path.

### Conversion goal

Reinforce legitimacy and data trust at the end of the page.

### What should NOT be included

- A sitemap.
- Empty links to future pages.
- Social icons added by convention.
- Membership, careers, franchise, press, or partner links without real destinations and operational reasons.
- A repeated promotional banner.
- A different email-capture form.

## Responsive and Interaction Priorities

### Mobile-first priorities

- Keep the problem, value proposition, development stage, and first primary CTA visible without excessive introductory content.
- Stack all comparison and benefit structures vertically in the intended reading order.
- Make interest controls easy to tap and understandable in seconds.
- Reveal the optional second interest only after a primary choice.
- Keep the primary CTA available on a long page without obscuring form fields, validation, or privacy context.
- Avoid carousels for essential information.
- Keep FAQ interaction accessible and preserve expanded content when validation returns the visitor to the form.

### Desktop priorities

- Preserve the same information order; desktop should not become a separate, denser narrative.
- Side-by-side structures may be used for the category gap, experience components, or known/unknown status only when reading order remains clear.
- Do not place a visually dominant image beside an understated value proposition.
- Keep the form width and field grouping focused rather than stretching the form across the viewport.

### Accessibility requirements for later design

- Use semantic heading order.
- Maintain visible focus states and keyboard access.
- Do not communicate selected interests, errors, required fields, or development status through color alone.
- Associate helper text and error messages with the correct controls.
- Announce successful submission and submission errors appropriately.
- Respect reduced-motion preferences.
- Use imagery and alternative text that do not overstate what the image proves.

## Content and Proof Governance

Before publication, every material statement should be classified as one of:

- **Confirmed fact:** Operationally verified and current.
- **Intended principle:** A standard Strike is designing toward.
- **Proposed feature:** Under active consideration but not final.
- **Unknown:** Not yet decided or verified.

The page should update as Strike moves through development:

1. Replace unknown location and timing language only after confirmation.
2. Add real facility, team, and local proof as it exists.
3. Remove generic examples when exact equipment and programming are known.
4. Add pricing only when total cost, inclusions, terms, and policies are ready to publish together.
5. Add event or tour CTAs only when those opportunities exist and can be fulfilled.
6. Add social proof only after genuine experiences occur and permission is obtained.

This governance prevents a pre-launch wireframe from quietly turning planning assumptions into public promises.

## Wireframe Validation Questions

Low-fidelity testing should determine:

1. Can visitors explain what Strike is intended to be after the hero?
2. Can they distinguish it from both an access-only gym and a fixed-format studio?
3. Do they understand that Strike is not open and that major details remain unconfirmed?
4. Is the reason to share an email clear before the form appears?
5. Do self-directed exercisers understand that independent training is a real part of the concept?
6. Do beginners and returning exercisers perceive a clear, low-pressure starting point?
7. Can visitors choose a primary interest in a few seconds?
8. Do they understand that a second interest is optional and limited to one?
9. Do they understand what communication they are permitting?
10. Do they understand that signup is not membership enrollment?
11. Does any secondary link or content element distract from the lead form?
12. Can mobile visitors return to the form easily after reading the FAQ?

## Final Structural Recommendation

The first Strike landing page should be a single-purpose, mobile-first journey from problem recognition to permissioned interest. Its strongest conversion argument is not price, urgency, facility scale, or an amenity bundle. It is a specific and credible proposition: Strike is being designed to make consistency easier by connecting open-gym freedom with clear, flexible guidance.

The page earns the conversion by:

- Explaining that proposition quickly.
- Showing how the proposed experience fits together.
- Helping visitors recognize their own needs.
- Being explicit about what is not yet known.
- Offering a concrete but restrained communication benefit.
- Asking only for first name, email, one primary interest, and an optional second interest.

Every section exists to improve understanding, relevance, trust, or completion of that one conversion. If a proposed content block does not support one of those jobs, it should not be added.
