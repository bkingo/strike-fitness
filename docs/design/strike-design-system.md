# Strike Fitness Visual Design System

**Design direction:** Grounded Momentum  
**Status:** Implementation-oriented visual source of truth for the pre-launch landing page  
**Document date:** October 2026  
**Strategic sources:** `strike-business-brand-brief.md`, `strike-landing-page-strategy.md`, `strike-landing-page-wireframe.md`, and `strike-refined-creative-direction.md`

## Purpose and Principles

This system translates the approved Strike Fitness creative direction into production-ready visual guidance. It does not change the business strategy, finalize a logo, or imply that the club, location, services, pricing, or member outcomes already exist.

The system should make the digital experience feel like supportive wayfinding: clear enough to reduce uncertainty, energetic enough to create momentum, and grounded enough to avoid pressure. The core visual behavior is **small, purposeful elements connecting and accumulating into a stronger whole**.

Every design decision should support five principles:

1. **Clarity before decoration.** The next step, current status, and information hierarchy should be immediately understandable.
2. **Momentum without pressure.** Energy comes from progression, rhythm, and confident action—not urgency, aggression, or spectacle.
3. **Capability with approachability.** The system must feel credible to experienced exercisers and welcoming to people beginning or returning.
4. **Warm structure.** Grids, repeated units, and consistent patterns provide order; warm color, human imagery, and conversational detail prevent sterility.
5. **Honest presentation.** Visual polish must never make proposed features look confirmed or stock imagery look like proof of an operating Strike facility.

Two business-brand traits must remain visible within those principles:

- **Candid:** Status, terms, uncertainty, and next steps are stated plainly. “Clear” is the visual expression of candor, not a replacement for it.
- **Energetic:** Energy appears through confident hierarchy, active photography, rhythm, and progression. Calm interaction behavior should not make the brand feel passive or spa-like.

---

## 1. Color System

### Palette Overview

The palette uses a deep green foundation, warm off-whites, a restrained olive support color, and one orange action accent. It avoids the black-and-red combat shorthand common in aggressive fitness branding while retaining enough visual strength for a serious training environment.

Bright and saturated color should remain scarce. The orange accent is most effective when most of the page is neutral.

### Core Brand Colors

| Color | HEX | Purpose | Use | Do not use |
|---|---:|---|---|---|
| **Deep Spruce** | `#173F3B` | Primary brand color; communicates stability, capability, and grounded strength | Header and footer fields, major headings, dark feature sections, key structural elements, selected navigation states, and dark button alternatives | As the default body-copy color on dark backgrounds; across every section; as a near-black replacement without maintaining visual hierarchy |
| **Sage Olive** | `#68745B` | Secondary brand color; adds natural warmth and a neighborhood, human quality | Restrained diagrams, non-text pathway markers, illustration details, and occasional section accents | For text on light or tinted backgrounds; as a competing CTA color; as broad fields or tactical styling |
| **Action Orange** | `#B84720` | Principal accent and CTA color; communicates action, optimism, and forward movement | Primary buttons, active controls, limited progress markers, and important wayfinding | As a large page background, for long passages of text, on every icon, or as decorative noise; never pair it with dominant black to create an aggressive fight-poster effect |

### Neutral Foundation

| Color | HEX | Purpose | Use | Do not use |
|---|---:|---|---|---|
| **Warm White** | `#FFFCF6` | Default page background | Main page canvas and spacious editorial sections | As the only background throughout a long page when section changes need clearer orientation |
| **Canvas Sand** | `#F7F3EA` | Alternate background | Section rhythm, grouped explanatory content, FAQ areas, and low-emphasis bands | To create many alternating stripes or make every module look boxed in |
| **Paper White** | `#FFFFFF` | Primary surface/card color | Forms, cards that need separation, overlays, and high-clarity content surfaces | As a stark full-page background when Warm White would better support the brand tone |
| **Soft Sage** | `#EEF3EE` | Tinted surface | Selected interest states, supportive information panels, process steps, and quiet success contexts | As a universal card fill or as the only signal for a selected or successful state |
| **Training Ink** | `#24302F` | Primary text color | Body copy, headings on light backgrounds, labels, form values, and icons requiring strong contrast | As a dominant full-page background; the system should feel grounded, not blacked out |
| **Slate** | `#5B6663` | Secondary text color | Supporting copy, metadata, helper text, dates, and captions | Below normal readable sizes, on tinted dark surfaces, or for required information that needs primary emphasis |
| **Boundary** | `#7E8783` | Standard functional border color | Input outlines, control boundaries, quiet card boundaries, and inactive controls | As the only indication of focus, selection, error, or disabled state |
| **Boundary Strong** | `#68716D` | Emphasized border color | Hovered fields, selected controls, stronger dividers, and controls that need more definition | Around every card or section; excessive outlining makes the experience feel like enterprise software |

### Functional Colors

| Color | HEX | Purpose | Use | Do not use |
|---|---:|---|---|---|
| **Action Hover** | `#A83E18` | Primary CTA hover/pressed state | Pointer hover and active feedback | As a separate brand accent |
| **Progress Green** | `#2F6B4F` | Success and confirmed-completion color | Successful form submission, valid completion, and confirmed positive status | To imply a proposed feature is confirmed; as the sole success indicator |
| **Alert Red** | `#8B2F2F` | Error and destructive-state color | Field errors, submission failure, and destructive actions if they are introduced later | For promotional emphasis, urgency, or fitness motivation |
| **Caution Amber** | `#8A5A00` | Warning or attention color | Non-blocking cautions and information that needs review | As a CTA substitute or to manufacture urgency |
| **Focus Gold** | `#F2B544` | High-visibility focus highlight and small progress accent | Focus-ring enhancement, dark-background wayfinding, and limited milestone details | For text on light backgrounds or as the only focus indicator |

### Approved Contrast Pairings

The following pairings meet WCAG AA contrast for normal text:

- Training Ink on Warm White: approximately **13.3:1**
- Training Ink on Paper White: approximately **13.7:1**
- Slate on Paper White: approximately **6.0:1**
- Paper White on Deep Spruce: approximately **11.6:1**
- Paper White on Action Orange: approximately **5.3:1**
- Paper White on Progress Green: approximately **6.3:1**
- Paper White on Alert Red: approximately **8.3:1**
- Boundary on Paper White: approximately **3.7:1**
- Boundary on Canvas Sand: approximately **3.3:1**

Action Orange with Paper White passes AA for normal text with practical tolerance. Production assets and browser-rendered states should preserve the specified value. Do not place Training Ink on Action Orange for body-sized text.

### Color Application Rules

- Use Warm White as the default canvas, with Canvas Sand or Deep Spruce creating occasional, purposeful section transitions.
- Reserve Action Orange for the page's one primary action system and a small number of progress cues.
- Use Deep Spruce for brand authority and structure; it should visually outweigh the accent without making the page dark.
- Keep Sage Olive supportive and non-textual on light surfaces. It should enrich the palette without becoming another action color.
- Never communicate selected, required, successful, warning, or error states through color alone. Pair color with text, an icon, a border change, or another clear state marker.
- When photography sits behind text, use a solid or highly controlled overlay and verify the actual image crop at every responsive size. Prefer placing critical copy on a solid surface.

### Semantic Color Roles

Implementation should use semantic roles rather than raw color names:

| Role | Approved color |
|---|---|
| Page background | Warm White |
| Alternate section background | Canvas Sand |
| Elevated surface | Paper White |
| Selected surface | Soft Sage |
| Primary text | Training Ink |
| Secondary text | Slate |
| Primary action | Action Orange |
| Primary action hover/pressed | Action Hover |
| Default control boundary | Boundary |
| Hovered or selected boundary | Boundary Strong |
| Keyboard focus on light surfaces | Deep Spruce |
| Keyboard focus on Deep Spruce | Paper White |
| Interaction success | Progress Green |
| Error/destructive | Alert Red |
| Warning requiring attention | Caution Amber |

Progress Green is reserved for interaction success, not for labeling confirmed business facts. Focus Gold may support focus or wayfinding on Deep Spruce, but it must not be the only focus indicator on a light surface. Decorative dividers may use a lighter warm gray than Boundary only when they do not define a control or communicate state.

---

## 2. Typography

### Typeface Recommendation

Use **Public Sans** as the primary and only required brand typeface.

Public Sans is an open-source, readily available web font with open letterforms, a broad character set, and a tone that is contemporary without feeling futuristic. It can carry substantial headlines, practical form guidance, policies, and navigation without splitting the brand into separate editorial and utility voices.

Use Public Sans for both the **heading typeface** and **body typeface**, as well as navigation, buttons, labels, and form text. Hierarchy should come from size, weight, spacing, and layout rather than a change of font family.

Recommended fallback category: a high-quality system sans-serif stack. The fallback should preserve clarity and approximate proportions rather than introduce a contrasting personality.

No secondary typeface is needed for the landing page. Adding one would create complexity without improving the approved direction. If a future long-form editorial need justifies a second face, it should be evaluated separately rather than added by default.

### Font Weights

- **400 Regular:** Body copy, descriptions, FAQ answers, and supporting information
- **500 Medium:** Secondary navigation, emphasized body text, and compact metadata
- **600 Semibold:** Buttons, form labels, status labels, and small headings
- **700 Bold:** Section headings and primary display text
- **800 Extra Bold:** Rare hero emphasis only; do not use for entire sentences or long headings

Avoid weights below 400 for body text. Avoid 900-weight display text, which can become visually aggressive.

### Heading Hierarchy

Sizes are recommended targets, not rigid values. Responsive scaling should remain controlled rather than creating extreme jumps.

| Style | Desktop target | Mobile target | Weight | Line height | Use |
|---|---:|---:|---:|---:|---|
| **Display / H1** | 60 px | 40 px | 700 | 1.06 | One concise hero headline |
| **H2** | 42 px | 32 px | 700 | 1.14 | Major section titles |
| **H3** | 28 px | 24 px | 700 | 1.22 | Module and subsection titles |
| **H4** | 21 px | 20 px | 600–700 | 1.3 | Card or step titles |
| **Eyebrow / category label** | 14 px | 14 px | 600–700 | 1.35 | Category labels and short wayfinding cues |
| **Development status** | 16 px | 15 px | 600 | 1.4 | Pre-launch status that must remain easy to notice |

Heading guidance:

- Keep the H1 concise and active. Favor natural title or sentence case.
- Use letter spacing near normal for headlines. Slight tightening may be used only at large display sizes.
- Eyebrows may use modest positive tracking. Avoid wide-spaced all caps that resembles tactical or athletic branding.
- Use 700 as the default maximum headline weight. Weight 800 is reserved for a single short emphasis of no more than three words and requires design review; it is not the default H1 treatment.
- Do not rely on font size alone for hierarchy; combine size, weight, spacing, and placement.
- Do not skip heading levels to achieve a visual treatment.

### Body and Utility Text

| Style | Recommended size | Weight | Line height | Use |
|---|---:|---:|---:|---|
| **Body large** | 19–20 px | 400 | 1.5–1.6 | Hero support copy and key explanatory passages |
| **Body default** | 17–18 px | 400 | 1.55–1.65 | Main page content |
| **Body small** | 15–16 px | 400–500 | 1.45–1.6 | Helper text, captions, and compact secondary content |
| **Form label** | 15–16 px | 600 | 1.35–1.45 | Persistent field labels |
| **Button text** | 16–17 px | 600–700 | 1.2 | Primary and secondary buttons |
| **Navigation text** | 15–16 px | 600 | 1.2 | Header anchor links |
| **Legal/support text** | 14–15 px | 400 | 1.5–1.6 | Privacy context and footer details |

Body-copy line length should generally remain between **55 and 75 characters**. Short explanatory text may be narrower. Avoid full-width paragraphs on desktop.

### Typographic Character

- Use sentence case for buttons, navigation, labels, and headings.
- Use short sentences and plain-language labels.
- Use numerals, milestones, and repeated labels consistently when showing sequence or progression.
- Use bold selectively to make scanning easier; do not create paragraphs with multiple competing emphasis styles.
- Do not use condensed athletic faces, stencil or varsity lettering, distressed treatments, metallic effects, delicate luxury serifs, or novelty rounded fonts.
- Do not turn “Strike” into a visual command through oversized all-caps typography.
- Public Sans remains the required interface and content face. Brand distinctiveness should come from the wordmark, composition, imagery, and the controlled progression motif rather than an additional web font.

---

## 3. UI Design Language

### Buttons

Buttons should feel solid, clear, and calm rather than explosive.

**Primary button**

- Action Orange background with Paper White text
- Minimum target height of 48 px; 52–56 px is preferred for the main landing-page CTA
- Horizontal padding should make the button feel generous without creating a banner
- Semibold or bold sentence-case label
- 8 px corner radius
- Optional simple directional icon only when it clarifies the action
- One primary button style should represent the same signup action throughout the page

**Secondary button**

- Transparent or Paper White surface
- Deep Spruce text and a visible Deep Spruce border
- Equal target height to the primary button
- Reserved for a legitimate second transactional action introduced in a later lifecycle stage
- Do not use it for landing-page learn-more, FAQ, or “how it works” actions; those remain text links

**Text link**

- Deep Spruce by default
- Underline by default in body copy, or another persistent non-color cue
- Hover should strengthen the underline or color; it should not cause layout movement
- Action Orange is reserved for button-like actions and should not be used for body-copy links

Button labels must describe the next step or benefit. Do not use generic “Submit,” premature “Join now,” or pressure language.

### Form Fields

- Keep labels visible above fields; placeholders do not replace labels.
- Use Paper White fields on Warm White or Canvas Sand.
- Default fields use a 2 px Boundary outline and an 8 px radius.
- Controls should be at least 48 px high with comfortable internal padding.
- Use Training Ink for entered values and Slate for supporting text.
- Hover may strengthen the border to Boundary Strong.
- Focus on light surfaces uses a 3 px Deep Spruce outline with at least 2 px visual separation from the control. Focus Gold is not used as the sole light-surface focus ring.
- Error states use Alert Red border, an error icon, and plain-language inline text connected to the field.
- Preserve valid entries after errors.
- Required and optional status must be written explicitly, not indicated only by an asterisk.
- Disabled fields should be rare. When necessary, use reduced contrast plus an explicit unavailable state; opacity alone is insufficient.

Interest choices use one standardized pattern:

- The required primary interest is a single-select radio group presented as full-width selectable rows.
- Each row contains the consumer-facing label and one short helper line; the entire row is clickable.
- The selected state uses Soft Sage, a 2 px Boundary Strong border, and a visible radio indicator.
- After a primary choice, reveal an “Add a second interest — optional” control. The second radio group excludes the primary choice and allows removal.
- On mobile, use compact rows rather than large feature cards. Maintain at least 8 px between separate targets.
- Reveal the optional group directly after the primary group and announce its availability to assistive technology.
- Never infer primary status from selection order or visual position.
- Treat the choices as research and relevance fields, not an amenity showcase. Do not add category-specific promotional imagery, feature icons, or unequal visual emphasis.

### Cards and Connected Modules

Cards should organize related information, not turn every paragraph into a separate tile.

- Default surface: Paper White or Soft Sage
- Default radius: 12 px
- Default card padding: 24 px on large screens and 20 px on small screens
- Use a quiet border before using a shadow
- Keep internal alignment and padding consistent
- Let related cards share a baseline, connecting rule, repeated marker, or sequence label when they describe progression
- Use varied composition sparingly to maintain a human quality
- On mobile, stack cards in the intended reading order

Avoid a dense “card wall,” floating feature tiles, isolated icon bubbles, and equal visual weight for every piece of content. The page should feel like a connected journey.

### Border-Radius Philosophy

Use moderate radii to communicate approachability without making the system playful or app-like.

- **4–6 px:** Small tags, compact status markers, and minor controls
- **8 px:** Inputs and standard controls
- **12 px:** Cards and medium modules
- **16 px:** Large form or feature surfaces
- **Fully rounded:** Reserved for small status pills or simple chips, not primary buttons or large content containers

Do not mix many radius values within one component family. Avoid both severe square corners across the whole interface and oversized “bubble” shapes.

### Borders

- Borders are functional: they define inputs, selection, grouping, and state.
- Use warm gray Boundary rather than cool technical gray.
- Standard content dividers should be thin and quiet.
- Selected or focused controls should increase both contrast and stroke strength.
- A short colored edge or repeated marker may identify a sequence, but it should not become an arbitrary decorative stripe system.
- Do not outline every section.

### Shadows

Shadows should be subtle and uncommon.

- Use a low, soft shadow only when elevation communicates a real relationship, such as a sticky header or elevated form surface.
- Prefer borders, spacing, and background shifts for ordinary separation.
- Keep shadow color neutral and low-opacity; avoid dramatic black drop shadows or colored glows.
- Hover elevation should be slight and paired with another cue.

### Spacing Philosophy

Use a **4 px base unit**. Approved spacing tokens are 4, 8, 12, 16, 24, 32, 48, 64, 80, 96, and 112 px. Components must select from these tokens rather than introducing intermediate values.

Spacing should communicate:

- **Room:** Generous section spacing reflects a usable, non-crowded experience.
- **Connection:** Tighter spacing joins labels, descriptions, and controls that belong together.
- **Progression:** Repeated intervals can show sequential steps or accumulated effort.
- **Priority:** Larger gaps separate major decisions; smaller gaps support quick scanning.

Do not use excessive whitespace that turns the page into a luxury editorial experience. Do not compress content into a dashboard-like density.

### Icons

- Use Lucide as the default functional icon family, with simple outlined icons, rounded joins, and a consistent 2 px visual stroke.
- Use 16, 20, and 24 px icon sizes. Do not mix libraries within one interface.
- Favor familiar functional symbols for direction, confirmation, information, and field states.
- Keep icons secondary to labels. Important actions and concepts must remain understandable without them.
- A custom visual family may use connected segments, measured intervals, or open paths.
- Avoid boxing gloves, fists, lightning bolts, flames, shields, crosshairs, bullseyes, weapons, anvils, hammers, impact bursts, and tactical badges.
- Avoid generic trophy, stopwatch, and flexed-arm symbols unless a specific functional context genuinely requires them.

### Image Treatment

Photography should show purposeful participation rather than fitness theater.

- Favor natural or lightly warm color grading with accurate skin tones.
- Use real ambient light and credible training environments; avoid dark nightclub lighting and fluorescent color casts.
- Show adults across ages, body types, genders, experience levels, and training preferences without making representation feel staged.
- Include individual focus, respectful coaching, comfortable proximity, and ordinary pauses between efforts.
- Use sequences, repeated viewpoints, or connected crops to suggest practice over time.
- Use medium and wider environmental crops alongside detail shots. Avoid physique-first cropping.
- Keep image corners aligned with the system's moderate card radius when images are contained.
- Captions should distinguish conceptual, stock, build-progress, and confirmed Strike imagery when that context matters.

Default contained-image ratios are 4:3 for environmental views, 3:2 for editorial/process imagery, and 1:1 only for compact people or detail cards. Each responsive crop must preserve a documented focal point. If text must overlay an image, use a Deep Spruce scrim strong enough for the actual text pairing to meet contrast at every crop; do not standardize an opacity without testing the source image.

Before Strike operates, stock photography must not imply that pictured people are members or that a pictured facility is Strike's completed club. Prefer honest founder, planning, equipment-selection, community-research, or actual progress imagery as it becomes available. Use explicit “conceptual” labels for renderings or images that could reasonably be mistaken for Strike proof; ordinary decorative stock does not need a bureaucratic caption when the surrounding copy makes no factual claim.

Avoid boxing and combat shorthand, bodybuilding poses, suffering imagery, yelling coaches, staged high-fives, forced group enthusiasm, transformation comparisons, and a dominant hero athlete who makes ordinary visitors feel like spectators.

The image library must also preserve serious-training credibility. Include usable equipment, legible training zones, independent effort, technique, and ordinary moments around racks, cables, free weights, cardio equipment, and open floor space. Warmth must not make Strike look like a passive wellness service or class-only studio.

### Section Transitions

- Alternate Warm White and Canvas Sand where a change in topic needs orientation.
- Use Deep Spruce for at most a small number of anchor sections, such as a trust or final CTA band.
- Use repeated markers, short connecting lines, numbered intervals, or aligned edges to carry momentum across sections.
- Keep transitions primarily horizontal and orderly.
- Use subtle asymmetry or an offset image to add humanity without breaking reading order.
- Avoid aggressive diagonals, torn edges, impact shapes, shattered textures, or decorative arrows with no informational role.

### Hover, Active, and Motion States

- Hover changes should be restrained: darken the action color, strengthen a border, reveal an underline, or add slight elevation.
- Active/pressed states should look physically settled, usually through a darker color and minimal downward movement.
- Selected choices must remain visibly selected after pointer movement.
- Motion should explain connection, progression, expansion, or state change.
- Typical transitions should be brief and calm, approximately 150–250 ms.
- Do not use bounce, shake, confetti, explosive reveals, continuous pulsing, or gamified streak effects.
- Respect reduced-motion preferences by removing nonessential movement and preserving immediate state changes.
- Anchor navigation should jump immediately rather than smooth-scroll when reduced motion is requested.

### Focus States

- Every interactive element needs a persistent, high-contrast keyboard focus indicator.
- On light surfaces, use a 3 px Deep Spruce outline with at least 2 px separation from the control.
- On Deep Spruce surfaces, use a 3 px Paper White outline; Focus Gold may be added as support.
- On Action Orange, use a 2 px Paper White inner outline plus a 3 px Training Ink outer outline with visible separation. The inner edge contrasts with the button and the outer edge contrasts with the light page surface.
- Focus indicators must not be clipped by overflow or hidden beneath sticky elements.
- Focus styling should be at least as visible as hover styling and should not depend on color alone when state could be ambiguous.

---

## 4. Layout

### Content Width

- **Primary page container:** Maximum width of 1200 px
- **Text-focused content:** Maximum width of 720 px
- **Lead form:** Maximum width of 600 px
- **Full-bleed backgrounds:** May span the viewport, but content remains aligned to the primary container
- **Outer gutters:** Use the responsive tier values defined below

The page should not stretch explanatory copy or form fields across wide displays.

### Grid Behavior

Use these shared responsive tiers:

| Tier | Viewport | Grid | Outer gutter | Column gap |
|---|---:|---:|---:|---:|
| **Small** | 0–639 px | 4 columns | 16 px; increase to 20 px when space allows | 16 px |
| **Medium** | 640–1023 px | 8 columns | 24 px | 20 px |
| **Large** | 1024 px and above | 12 columns | 32 px | 24 px |

The primary container remains capped at 1200 px. Typography interpolates between its mobile and desktop targets across the Medium tier and reaches the desktop target at the Large tier.

- Use a 12-column desktop grid, an 8-column intermediate grid, and a 4-column mobile grid as planning frameworks.
- Grid columns should organize alignment, not force every section into the same composition.
- Related modules should share edges and spacing intervals.
- The experience sequence may use four equal steps on wide screens, but reading order must remain clear when it stacks.
- Side-by-side content should become vertical before either side becomes cramped.
- Keep the primary CTA and form visually dominant over supporting cards, images, and links.

### Section Spacing

- Standard major sections: 96 px vertical padding on Large, 80 px on Medium, and 64 px on Small
- Emphasized hero or final conversion sections: up to 112 px on Large and 80 px on Small
- Compact status, trust, or transition sections: 48–64 px
- Closely related subsections: 48 px
- Internal module spacing: 24 or 32 px

Use the smallest appropriate variant. Do not apply major-section spacing mechanically to every block on the long landing page.

### Desktop Layout

- Preserve the mobile information order rather than creating a separate desktop narrative.
- Use controlled two-column layouts for the hero, category gap, known/developing status, or image-and-copy pairings.
- Text should remain the primary driver in the hero. Imagery must not overpower an understated proposition.
- Keep navigation minimal and the primary CTA visible.
- Center or deliberately offset the lead form, but do not stretch it across the page.
- Use negative space to create confidence and usable rhythm, not exclusivity.
- Keep the hero and header usable when the CTA label wraps or text is enlarged; do not reduce type below its defined minimum to force one line.

### Mobile Layout

- Keep the development status, problem, proposed answer, and first CTA visible early.
- Stack comparison, process, benefit, and trust modules in the intended reading order.
- Make all controls easy to tap, with a minimum 44 × 44 px target and a 48 px preferred control height.
- Keep interest-choice labels and helper text visible without separate modal explanations.
- Use a restrained sticky CTA only if testing shows it improves navigation to the form; it must disappear near the form and never obscure validation or privacy text.
- A sticky CTA may be no taller than 64 px excluding device safe-area inset. Hide it whenever the form, consent disclosure, validation summary, or confirmation state is visible.
- Avoid carousels for essential content.
- Do not hide important trust or status information behind interactions.

### Responsive Behavior

- Scale typography fluidly within the defined ranges; avoid abrupt display-size jumps.
- Let layouts reflow based on content fit rather than device labels alone.
- Maintain consistent reading order in the document and visual layout.
- Collapse multi-column modules before copy, buttons, or controls become narrow.
- Crop photography intentionally at each major aspect ratio; do not rely on one desktop crop.
- Keep primary actions full-width on narrow screens when that improves tap clarity. Secondary links should remain visually subordinate.
- Test common zoom levels and text enlargement. Content must reflow without horizontal scrolling at 400% zoom for typical desktop viewport conditions.
- Test at 320 px CSS width, with long labels and browser text enlargement. No primary action, status label, or interest choice may depend on truncation.

### Conversion Layout Rules

- All primary anchor CTAs point to one canonical lead form and preserve entered values.
- Do not render duplicate independent forms. If a hero-form variant is tested, move or reveal the same form experience rather than creating unsynchronized records or validation.
- Use a visible-on-focus “Skip to main content” link and a “Skip to signup form” link on the long landing page.
- Anchor destinations need scroll clearance below any sticky header and must receive logical keyboard focus when appropriate.
- Form placement and FAQ order must follow the approved conversion wireframe or an explicitly documented test variant; visual styling must not silently change the funnel architecture.

---

## 5. Accessibility

The production website should target **WCAG 2.2 Level AA** as a baseline.

### Color Contrast

- Normal text requires at least 4.5:1 contrast.
- Large text requires at least 3:1, though stronger contrast is preferred.
- User-interface components, control boundaries, focus indicators, and meaningful graphics require at least 3:1 against adjacent colors.
- Verify actual combinations in production, including hover, disabled, error, selected, and image-overlay states.
- Do not use Sage Olive, Focus Gold, or light neutral colors for body text on light backgrounds.
- Do not communicate meaning through color alone.
- In forced-colors or high-contrast modes, preserve native control boundaries, focus, selection indicators, and error markers rather than forcing brand fills.

### Typography and Readability

- Default body text should be 17–18 px with generous line height.
- Do not place long passages in all caps, italics, centered alignment, or narrow columns.
- Preserve user zoom and text-resizing behavior.
- Keep line lengths controlled and paragraph spacing visible.
- Use semantic heading order and meaningful link text.
- Avoid thin font weights and low-contrast helper copy.

### Buttons and Links

- Provide a minimum 44 × 44 px pointer target; larger targets are preferred for primary actions.
- Use descriptive labels that communicate outcome or destination.
- Distinguish links from surrounding text with more than color.
- Ensure hover, focus, active, disabled, loading, success, and failure states are visually distinct.
- Loading states must keep the button label understandable and prevent accidental duplicate submission without trapping focus.

### Form Fields

- Associate every input with a persistent programmatic label.
- Connect helper text and error messages to their fields.
- Identify required and optional fields in text.
- Preserve entries after validation failure.
- Use appropriate input purpose and autocomplete behavior when implemented.
- First name and email fields require the appropriate autocomplete and mobile input behavior in the first release.
- Interest choices must be keyboard operable and expose selected state to assistive technology.
- Announce submission success and failure appropriately.
- Submitting state must expose busy status without moving focus. Success uses a polite status announcement; a blocking integration failure uses an assertive error announcement and a clear retry path.
- Move focus only when it helps the user recover or understand a state change; do not unexpectedly reset it.

### Focus States and Keyboard Use

- All interactive elements must be reachable and operable by keyboard.
- Focus order must follow the visible reading order.
- Focus indicators must remain visible against every surface and must not be removed.
- Sticky navigation must not cover focused elements or anchor destinations.
- Accordions such as FAQ items must expose expanded/collapsed state and support standard keyboard behavior.
- FAQ controls remain buttons with visible text labels; expansion state cannot be communicated only by a rotating icon.

### Error and Status States

- Pair Alert Red with a clear icon, concise heading or label, and actionable message.
- Explain what happened and how to correct it; avoid blame or alarmist language.
- Place field-level errors next to the relevant field and provide an error summary when multiple failures make that useful.
- Do not clear valid data.
- Distinguish backend failure from validation failure and do not show a success state until the lead record is accepted or reliably queued.
- Success messaging should be calm and specific. Avoid confetti or exaggerated celebration.
- Development status, proposed features, and confirmed facts must use explicit labels, not color coding alone.

### Content Status Labels

Use one neutral status-label component to distinguish:

1. **Confirmed fact**
2. **Intended principle**
3. **Proposed feature**
4. **Not yet known**

Each variant uses explicit text and, where helpful, a distinct icon or border treatment. Do not use Progress Green to label confirmed facts, Caution Amber for ordinary pre-launch uncertainty, or color alone to distinguish variants. Apply the component consistently to the development-status message, known/developing module, renderings, and any named equipment or programming detail that could otherwise appear confirmed.

### Images and Motion

- Write alternative text according to the image's purpose; decorative images should not create redundant announcements.
- Do not use alternative text to overstate what stock or conceptual imagery proves.
- Avoid text embedded in images.
- Respect reduced-motion preferences.
- Do not autoplay distracting motion or video, and provide controls for any time-based media introduced later.

---

## 6. Brand Expression

### How the System Reinforces Grounded Momentum

**Grounded**

- Warm White, Canvas Sand, Deep Spruce, and restrained olive tones create stability without the severity of black.
- Clear typography, visible labels, practical form patterns, and honest status treatment communicate preparedness and respect.
- Moderate radii, limited shadows, and tactile warmth keep the experience human without making it soft or sentimental.

**Momentum**

- Action Orange makes the next action visible without turning the full page into a promotion.
- Repeated intervals, connected modules, milestones, and sequential layouts show how manageable actions build.
- Controlled hover and state transitions reinforce continuation rather than spectacle.
- The visual journey moves from recognition and relief toward clarity, confidence, and a practical next step.

**Candid**

- Explicit status labels, direct form expectations, and plain-language disclosures make uncertainty understandable without turning the page into a warning.
- Visual hierarchy gives confirmed information and unknowns appropriate weight without disguising either.

**Energetic**

- Energy comes from active language, purposeful photography, confident scale, and rhythmic progression.
- It does not depend on aggressive weight, constant motion, orange saturation, or high-intensity fitness theater.

**Capability**

- Substantial headings, strong contrast, disciplined grids, and precise states support serious training credibility.
- Independent training and coached guidance should receive balanced visual treatment so neither audience feels secondary.
- Guidance by default is a cross-cutting service promise, not a special-interest feature. Visual hierarchy should show a clear starting path throughout the experience while keeping optional higher-touch coaching distinct.
- Space, consistency, and predictable interactions make the interface itself demonstrate the operational values Strike intends to uphold.

**Approachability**

- Open letterforms, readable sizing, warm backgrounds, generous controls, and realistic photography reduce intimidation.
- Human variation in composition and imagery prevents the system from feeling corporate or clinical.
- Calm error handling and explicit low-commitment language reinforce support without pressure.

**Neighborly character**

- Local details should enter the system only when a location and relationships are real.
- Real people, progress, planning, and community participation should gradually replace generic conceptual material.
- The system should feel accountable and useful, not like a national campaign with a location name inserted.
- Until a location exists, founder rationale, planning work, listening activity, and real development progress are stronger signals of accountability than generic neighborhood imagery.

### Signature Progress Motif

Use one primary visual behavior: **measured units align, repeat, and continue**. It may appear as a short sequence of segments, numbered intervals, or an open path that continues beyond a milestone.

- Use the motif only when it clarifies sequence, accumulation, navigation, or status.
- Keep geometry horizontal or gently stepped, with rounded or neutral joins.
- Do not depict collision, impact, targets, explosive convergence, or two forms striking one another.
- Do not combine more than one progress treatment within a section.
- Decorative use should remain secondary to content and should not appear in every section.

### Visual Characteristics to Avoid

Do not use:

- Dominant black-and-red palettes
- Fluorescent performance colors or nightclub lighting
- Boxing, combat, martial-arts, military, tactical, or fight-promotion cues
- Literal hammers, anvils, construction tools, sparks, impact bursts, shattered surfaces, or demolition imagery
- Lightning bolts, crosshairs, bullseyes, shields, fists, aggressive slashes, or weapon-adjacent marks
- Ultra-condensed athletic, stencil, varsity, distressed, metallic, or futuristic typography
- Oversized all-caps commands
- Bodybuilding, physique worship, supplement-brand aesthetics, or transformation imagery
- Pain, punishment, coach-yelling, collapse, or sweat-as-suffering imagery
- Forced team huddles, generic high-fives, or “fitness family” clichés
- Overly muted spa and wellness styling that removes training credibility
- Luxury-editorial styling that makes the club feel exclusive
- Sterile dashboards, excessive cards, dense data displays, or enterprise-software aesthetics
- Rainbow feature coding that makes the experience look like disconnected products
- Decorative progress graphics, arrows, or motion that do not clarify information
- Fake scarcity, countdowns, pulsing CTAs, or urgent promotional color fields
- Visual treatment that makes unconfirmed concepts, stock imagery, or renderings appear to be established facts

### Wordmark and Name Guardrails

Until a final identity is approved, use a provisional text wordmark in Public Sans 700:

- Set “Strike Fitness” in title case, not full uppercase.
- Keep letter spacing near normal; do not italicize, shear, compress, distress, outline, or add impact effects.
- Keep “Fitness” visible in primary first-touch contexts so “Strike” is not interpreted in isolation.
- Do not place the wordmark in a crest, shield, fight badge, target, or apparel-style lockup.
- Maintain clear space equal to at least the cap height of the “S” and never reproduce the wordmark below 120 px wide digitally.

The final wordmark should be tested without explanatory copy for associations with boxing, combat sports, tactical products, labor action, and high-intensity boutique fitness before replacing this provisional treatment.

### Landing-Page Component Set

The first implementation should include one approved version of each:

- Minimal header and responsive header CTA
- Development-status label or bar, with a rule preventing duplicate status treatments
- Primary button, text link, and loading button
- Text input with default, hover, focus, valid, error, disabled, and unavailable states
- Primary-interest radio rows and optional second-interest disclosure
- Consent and privacy disclosure block
- Known/developing trust module using content status labels
- FAQ accordion
- Sticky mobile CTA, only if validated
- Form validation summary
- Submission loading, success, existing-profile update, and integration-failure panels

Components use the tokens and state behavior in this document. New visual variants require a demonstrated content or interaction need, not preference.

### Decision Filter

Before approving a visual treatment, ask:

1. Does it make the next step clearer?
2. Does it show progress as manageable, connected effort?
3. Does it welcome someone newer to fitness without weakening credibility for an experienced exerciser?
4. Does it allow both individual focus and comfortable human connection?
5. Is the energy active and optimistic without becoming loud or pressuring?
6. Could it be mistaken for boxing, bodybuilding, punishment, elite performance, or a promotional chain-gym campaign?
7. Does it accurately distinguish confirmed facts, intended principles, proposed features, and unknowns?
8. Does it feel like a dependable local training club rather than a generic fitness brand?

---

## Major Design Decisions

- **One grounded foundation:** Deep Spruce and warm neutrals establish trust, readability, and training credibility without aggressive black.
- **One action accent:** Action Orange identifies primary actions and meaningful progress; it is intentionally used sparingly and meets normal-text contrast with Paper White.
- **One type family:** Public Sans provides a clear, capable, and approachable voice across display, body, navigation, and forms.
- **Moderate, functional UI styling:** Generous controls, restrained radii, quiet borders, and minimal shadows make the experience welcoming but serious.
- **Connected rather than card-heavy layouts:** Repeated units, aligned modules, and measured intervals express progress as accumulation.
- **Mobile-first clarity:** The same problem-to-action journey is preserved across screen sizes, with strong reading order and accessible controls.
- **Accessible by default:** High contrast, visible focus, explicit states, readable type, and robust form feedback are part of the brand experience.
- **Human, honest imagery:** Photography emphasizes purposeful participation and real progress while clearly distinguishing conceptual material from actual Strike proof.
- **Firm visual boundaries:** Combat, punishment, transformation, nightlife, tactical, bodybuilding, false urgency, and decorative progress clichés are excluded.
