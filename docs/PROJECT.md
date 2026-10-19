# Funnel project record

## Second-section layout refinement — 19 October 2026

The user's screenshot identified uneven process arrows and weak spacing in the navy section. This update replaces the text-glyph arrows and top-rule layout with four circular outline-icon nodes, identical SVG arrowheads and connectors positioned from node centres. Desktop stage labels share a top edge; mobile uses a vertical column with centred downward connectors. The three problem rows gain matching outline icons in restrained rounded-square shapes, consistent padding and improved heading alignment. A lightly tinted, bordered process panel groups the workflow and preserves its exact outcome disclaimer. The icons are decorative and hidden from assistive technology; the semantic ordered list still communicates the stages.

All original section paragraphs, offer terms and process labels remain. Source comparison confirms that all markup, scripts and copy outside this section are unchanged. No libraries, generated images, competing actions or continuous motion were added. The existing reduced-motion and progressive-reveal behaviour is preserved.

The final HTML passed **116 targeted assertions** at 320, 360, 390, 430, 540, 768, 800, 801, 1024, 1440 and 1920 CSS pixels. Actual browser geometry verifies equal horizontal node spacing/connector lengths, shared node and label alignment, arrow clearance, and equal vertical spacing/centred arrows on mobile. Checks also cover containment, overflow, preserved text, SVG accessibility, script errors, reduced motion and no-JavaScript visibility. Axe WCAG A/AA scans of the section report zero automated violations at all eleven widths. These are focused checks for this change; the preceding 232-check whole-page record remains the earlier validation, not a rerun of this version.

Actual rendered close-ups: `previews/process-desktop.png` and `previews/process-mobile.png`. The full-page desktop/mobile screenshots are refreshed, and `verification-process-2026-10-19.json` records the tested HTML hash. The changes remain on the review branch. No merge, production deployment, booking destination, pricing, portrait or launch setting was changed.

## Buyer-relevance and evidence review — 19 October 2026

Source: the clean, current `review/funnel-design-refinements` branch at `2b3d69be9b400a5fcf3e618f3d4a45a68302a3e5`. It already contained the portrait, supplied Calendly URL and scroll reveals. No unrelated local edits were present. The new attachment was a text design brief; no PDF, uploaded HTML, separate photo, Loom, case evidence or teaching/creative artifact was accessible. The PDF description in the brief was treated as guidance, not as an inspected document or a live pagination defect. No conflicting uploaded HTML was overwritten. Earlier dated entries below are history, not current public content or current asset status.

The implementation refines the existing single file and reuses its portrait, fonts, offer and optional-media code. It removes the public internal status label and header founder subline, makes the hero owner-focused while keeping the 30-unique-enquiry/15-live-day commitment prominent, replaces the capability list with problem-to-action situations and a semantic process, and adds a readable illustrative qualification/handoff workflow. The sample is explicitly labelled as illustrative, not client results. No customer outcome, client count or testimonial is fabricated. Actual role-based credibility comes from the user's current brief; see `CLAIMS.md`.

The former fit cards and black founder/quotation block become a compact checklist and lighter founder introduction. The large self-authored quotation is removed; its admissions-feedback mechanism is explained in the approach. Prices are shown in a calmer management-plus-additional-costs layout, all visible before booking. The existing management-fee guarantee paragraph is preserved verbatim. The eight native FAQs separately address qualification, enquiries versus enrolments, scope, admissions responsibility, the 15/30-day windows, fees, missed targets and setup failure. Repeated explanations were tightened. No prices, media/software periods, future price stages or confirmed client results were invented.

The visual system uses white, warm light paper and a single navy section. The original Arial/Helvetica and Georgia families remain; the original portrait's encoded bytes are unchanged. The image has a simple frame and one readable caption. Core text is 17–18px, terms/answers 16px and supplementary cost descriptions at least 15px. Mobile puts the offer/CTA before a compact portrait and stacks the process. Reveals are progressive 300ms/8px entrances with a slight fade from 95% opacity, once per element. An earlier stronger fade was corrected after investigating transient text contrast; the first frame now has its own passing contrast check.

All four booking placements retain the exact supplied Calendly destination. They are native links, so both calendar navigation and FAQs work without JavaScript. The header CTA is hidden through 540px; hero, approach and final placements remain. The final call covers courses/fees/seats/intake timing, the admissions process and pilot suitability, with no purchase or immediate decision required merely to book. No full audit or free customised strategy deliverable is promised. The optional early video insertion point remains hidden without a genuine approved URL; no empty player is published.

### Verification

Final validation passed **232 assertions** against the actual HTML in Chromium. Tested widths: 320, 360, 390, 430, 540, 768, 800, 801, 1024, 1440 and 1920 CSS pixels. Checks cover balanced HTML, unique IDs/ARIA/anchor references, one H1, five visible main sections, exact portrait decoding and preserved bytes/fonts/guarantee, visible pricing/scope, absence of internal status wording, hero order/crop, process stacking, readable type, no overflow before/after scroll, no JavaScript errors or automatic external resource requests, and all scroll targets reached.

Axe WCAG 2/2.1 A/AA scans reported zero automated violations at all eleven widths and with all FAQ answers expanded. A separate contrast scan passed with a reveal paused on its first frame. Keyboard checks cover skip-to-main focus, visible focus at all four calendar links, all eight FAQs opening with Enter/closing with Space, and summary touch targets of at least 44px. Each calendar placement navigated to the exact supplied URL using an intercepted response, without creating an appointment. Tests also cover one-time 300ms animation, reduced-motion/no-observer/no-JavaScript fallbacks, real native calendar navigation without JavaScript, valid/unsafe settings, launch indexing guards without the removed badge, portrait-error fallback, hidden missing/unsupported video and click-to-load allowed video with no autoplay and a responsive iframe.

Desktop and mobile screenshots in `previews/` are actual Chromium renders of the final HTML and were visually reviewed. They are available through GitHub to avoid relying on workspace download links. The validation record includes the tested HTML hash. Test-only tooling and temporary image separation were kept outside the checkout; no runtime dependency or build was added. These checks do not establish campaign results, complete accessibility certification or cross-browser parity; Firefox, Safari and real devices were not exercised.

### Current evidence and launch checklist

- [x] Remove all public internal review/status labels, preserve the single HTML and keep the existing review branch.
- [x] Keep prices, conditions, one-course/intake scope and the enquiry-versus-enrolment distinction clear.
- [x] Preserve the supplied Calendly link; test all placements and no-JavaScript navigation using interception.
- [x] Maintain the internal claim register and a clearly labelled illustrative workflow without pretending it is outcome proof.
- [ ] Verify actual Calendly event availability and duration. A current direct HTTPS attempt was blocked by the environment proxy: CONNECT HTTP 403. No calendar booking was made.
- [ ] Supply a genuine Loom embed URL and any approved poster/transcript if video is wanted.
- [ ] Supply permission-cleared case evidence or teaching/creative material, including ownership, country, date range, actual role and limitations. Approve any company/profile verification link.
- [ ] Confirm final qualification/counting, setup deadline, media/software coverage, interruption and refund procedures before commercial launch. Existing terms are shown honestly without filling unresolved facts.
- [ ] Set the actual canonical domain and authorise publication separately. `readyForLaunch` remains false and robots remain `noindex, nofollow`; no Vercel protection, merge or production deployment was changed. The historical Vercel scope issue was not retested.

## Calendly and scroll update — 15 October 2026

The user supplied `https://calendly.com/imhussain00112/free-growth-strategy-call`. It is configured in `bookingUrl` and enables both existing booking controls. The approved intake-review CTA wording is retained. No calendar embed, tracker, new dependency or automatic Calendly request is added. The event's availability and duration have not been independently verified: a read-only HTTPS check was blocked by the environment proxy with CONNECT HTTP 403. No appointment was created.

Individual introductions, service rows, fit cards, the founder principle and closing content now animate once when entering view. The 620ms entrance uses an 18px upward movement and a restrained fade from 80% opacity. Paired rows/cards have a 70ms offset. Elements remain fully visible before JavaScript applies the entrance class; missing IntersectionObserver leaves normal content. Reduced motion skips observation and disables animation. The effect finishes without retaining a transform, preserving card hover behaviour.

All 58 targeted Chromium assertions passed, covering 320/390/768/1024/1440px layouts, no horizontal overflow before or after animation, both enabled booking controls and their exact intercepted navigation destination, keyboard focus, one-time scroll animation, completed-animation hover, reduced motion, JavaScript-disabled FAQ/content, unsupported IntersectionObserver, portrait decoding, and unchanged portrait/pricing/guarantee/qualification terms. Updated desktop and mobile screenshots were visually checked. The earlier 101-assertion accessibility/layout review below records the preceding version; it was not rerun in full for this update.

Booking URL supply is resolved. Live calendar verification, Loom, optional poster/transcript, canonical URL and the remaining commercial launch approvals stay open. `readyForLaunch` remains false and indexing remains disabled. Changes stay on `review/funnel-design-refinements`; no merge or deployment is performed.

## Review update — 15 October 2026

Source inspection found `main` at `6e7cbe51cfdb5d653a46611ff7a285c51037a022`, containing only the initial README. The existing single-file funnel is on GitHub's `funnel-v1` at `28373073777de3520557d442e20b19fd70de2c6b`. This update branches from that existing funnel onto `review/funnel-design-refinements`. No uploaded HTML or separate portrait file is accessible in this session; there is no uploaded version available to compare. The already embedded portrait is available, decodes correctly, and its bytes are preserved exactly.

The source already contained the requested section palette, split hero, founder copy, restrained outline icons and reduced-motion behaviour. Those are retained. This pass makes Ahmad's identity primary in the masthead with Visionary Co. as the supporting founder line, integrates the photograph into a navy frame and caption, improves supporting text sizes and FAQ states, and confines card hover movement to devices with a precise pointer. An unavailable optional portrait override now falls back to the original image instead of removing the photograph.

The original Arial/Helvetica and Georgia font declarations, four prices and budget descriptions, management-fee guarantee, and all qualification/service/refund FAQ terms are preserved verbatim. The offer remains qualified course enquiries, with no paid-enrolment guarantee. Credibility stays non-numerical and tied to Ahmad's experience in Pakistan; no personal/company client count is asserted.

Actual Chromium checks passed 101 assertions. Layouts were exercised at 320, 360, 390, 480, 640, 768, 800, 801, 1024, 1440 and 1920 CSS pixels: no horizontal overflow or offscreen main content; copy precedes the compact portrait through the tablet breakpoint; desktop has copy left and photograph right. Full-page and hero screenshots at 390px and 1440px were visually reviewed. The portrait displays without broken assets or facial clipping. The default page makes no external resource requests and produced no JavaScript errors.

Axe-core WCAG 2/2.1 A/AA scans reported zero automated violations at each width. Keyboard checks covered the skip link, visible focus, all three FAQ disclosures with Enter/Space, and 44px summary touch targets. Both booking controls were tested with an intercepted HTTPS test destination, without opening a real calendar or making an appointment. Invalid/missing booking URLs remain disabled and keep the page unindexed. Reduced motion disables the relevant animation/transitions; all five sections, the embedded portrait and native FAQ remain usable with JavaScript disabled. Optional portrait failure restores the embedded image. A configured video was tested using an intercepted embed: no iframe/provider request before activation, responsive frame after activation and no autoplay permission/parameter. An unapproved video host remains hidden. Test fixtures and axe were kept outside the checkout; the site still needs no dependencies or build.

Booking, Loom, transcript/poster and canonical URL remain missing. Booking buttons remain honestly disabled; the video block and play control remain hidden. Numerical credibility needs confirmation of count and whether it is personal or company experience. The previously recorded commercial launch requirements remain open. Actual calendar delivery and actual video playback cannot be verified until their links are supplied. Automated checks do not replace human accessibility review or cross-browser testing; only Chromium was exercised here.

This review does not change Vercel access or deploy the page. The earlier Vercel scope issue was recorded by the existing project notes and was not re-tested in this environment. No merge, production deployment or indexing activation was performed.

## Direction recorded 14 October 2026

Identity: Ahmad Hussain — Founder of Visionary Co. Audience: owners and admissions decision-makers at independent Canadian training institutes. One primary action: a 20-minute intake-review call. Initial scope: one selected course and one upcoming intake, proposed for final confirmation.

Target: 30 unique qualified course enquiries in 15 live advertising days after setup and launch. Management period: 30 live advertising days. The CAD650 management fee is separate from CAD500 setup, CAD2,000 media budget and estimated CAD150 software allowance. Media and software periods remain unconfirmed.

The 15–20-day draft wording is excluded from the page. No internal future pricing stages are published. Proposed qualification and counting terms require review before launch. The institute's nominated admissions contact handles student conversations, eligibility and closing.

## References and adaptations

`https://musakhana.com/` was inspected visually in a browser. Its current page uses Inter-style bold sans-serif typography, centred hero copy, a contained text width, dark/gold colour treatment, a roofing background video, generous section spacing and a linear offer-to-call flow. It does not currently show a distinct VSL player in the inspected hero.

Adopted ideas: clear type hierarchy, constrained reading widths, purposeful spacing, a compact linear funnel and one commercial action. Adaptations: original copy for institute owners, light/black sections with the approved blue palette, founder credibility in place of invented case studies, visible separate costs, and an optional click-to-load explanatory video below the hero copy. No roofing imagery, source copy, source code, scaling claims or source guarantee is copied.

`https://www.visionarycodigital.com/` was inspected through page text and a browser screenshot. The current homepage uses dark/gold styling and serif headings. The funnel follows the black/white/blue direction supplied in this conversation, retaining founder/agency identity and a restrained serif treatment for the working principle. Homepage statistics, testimonials, portfolio claims and the existing founder image are not automatically imported or approved as proof.

The user asked for implementation after explaining the adaptation. A single-file version is being built; the reference and asset set can still evolve. The supplied reference is not treated as evidence of conversion performance.

## Asset register

| Input | Status |
| --- | --- |
| First design reference | Inspected and adapted |
| Additional design references | Open |
| Selected founder photo | Supplied WhatsApp portrait; approved for this edit, optimised to embedded WebP and placed in hero without retouching |
| Approved video and poster | Pending; optional block hidden |
| Actual transcript | Pending; omitted |
| Canadian case studies | None established |
| Testimonials/work examples | No publication-approved assets supplied |
| Booking URL | Supplied Calendly URL configured in both booking controls; live calendar verification blocked by the environment proxy |
| Final canonical URL | Pending |
| Tracking/pixels | Not approved or added |
| Numerical client claim | Unconfirmed; non-numerical personal experience used instead |

## Refinement decisions

The current GitHub `funnel-v1` HTML was the working source and matched the local file before this revision. No conflicting uploaded HTML was supplied. The supplied portrait file was available despite the attachment-path error in the user message.

The five-section funnel and original fonts are retained. White introduces the founder and offer; deep navy distinguishes the services; a light suitability section supports scanning; near-black gives the personal working principle emphasis; white returns for costs and the final call. Text colours were checked against their actual section surfaces.

The desktop hero places copy and the booking action on the left, with Ahmad's supplied portrait on the right. Mobile places the offer and CTA before the image, limiting the portrait width to 292px at common phone sizes and 265px at the smallest breakpoint. CSS cropping removes excess headroom while retaining the face. The photograph was compressed from 81,064 bytes to 35,418 bytes, with no facial alteration, generated content, retouching or filters. The complete HTML is 86,934 bytes.

Copy now uses Ahmad's first-person voice while recognising Visionary Co.'s delivery team and the institute's admissions responsibilities. The 15-live-day qualified-enquiry target, separate 30-live-day management period, itemised costs and management-fee guarantee remain intact. No paid-enrolment promise or unconfirmed numerical experience claim is introduced.

Decorative slash labels are removed. A small set of consistent outline SVGs explains the services and relevant experience. The same 20-minute booking action appears in the hero and closing section; it has no invented destination. The missing Loom remains hidden, with no visible non-functional play control.

Brief movement introduces the hero and selected sections. Content is visible before animation and without JavaScript. Reduced-motion preferences disable animations, transitions and hover movement. FAQ summaries have a minimum 44px target; enabled buttons have visible focus, hover and pressed states.

## Launch requirements

- Confirm the selected course/intake scope and final qualification/counting method.
- Approve the setup deadline; the seven-business-day suggestion remains a proposal and is not published.
- Confirm media and software budget coverage periods and selected tools.
- Approve final interruption, responsibility and refund procedures.
- Verify the supplied Calendly event's live availability, duration and intended audience without creating an unwanted appointment.
- Supply the actual Loom URL and any approved poster/transcript if video is wanted.
- Confirm the proposed numerical client claim and distinguish personal experience from the agency's company record before adding it.
- Review remaining references and final copy.
- Confirm GitHub-to-Vercel project linking, deployment target and staging protection.
- Complete available browser verification; record unavailable checks precisely.
- Set the canonical URL and `readyForLaunch` only after the required inputs are resolved.

## Access and delivery

GitHub repository: `ahmadhussainbiz/ahmad-institute-funnel`. Read and push permissions were verified. The repository is public. Preserve `main` while reviewing a dedicated branch. Publish no private records or credentials.

Vercel profile authentication works. The account's scoped team and project reads returned HTTP 403, with the provider reporting that the connection is not authorised for the requested project scope. The mapped Vercel CLI fallback is unavailable in this environment. No Vercel project was created, no deployment was made and no protection setting was changed. Resolve project-scope access before preparing a Vercel preview; do not treat a profile read as deployment permission.

The complete HTML and handover files are maintained on the `funnel-v1` review branch. The previous remote HTML was compared with the local source before refinement and matched exactly. `main` is preserved.

## Validation record

Refined-file checks passed on 14 October 2026: balanced HTML, exactly five main sections, one primary booking action with two consistent placements, unique IDs, valid ARIA/anchor targets, inline resource structure, responsive/focus/reduced-motion rules, preserved fonts, correct offer windows and honest default video/booking states. The embedded image decodes correctly as a 731 × 1280 WebP and matches the visually inspected optimised portrait. JavaScript syntax passed. Fourteen isolated behaviour checks passed for both booking controls, URL safety, indexing guards, optional-image error handling, click-to-load media, reduced-motion preferences and one-time entry animation. Ten main text/CTA colour combinations exceed a 4.5:1 contrast ratio.

These are source and isolated behaviour checks, not a browser accessibility certification. The managed local preview workflow requires a browser-control capability not available in this environment, so no local browser QA was claimed. A Vercel preview is blocked by the project-scope access error. No real booking destination has been supplied or verified.

Smallest remaining manual layout check: download `index.html`, open it in a browser, inspect a desktop width and 390px mobile width, open each FAQ and confirm there is no horizontal overflow. With a real booking URL configured, confirm that the booking button opens the intended calendar; do not create an unwanted appointment. Optional media should be checked only after approved assets are supplied.
