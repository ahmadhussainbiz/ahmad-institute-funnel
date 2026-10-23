# Ahmad Institute Funnel

A founder-led enrolment-pilot review page for Ahmad Hussain and Canadian training institutes, course providers and independent educators. The website is a single `index.html`, including the approved portrait, CSS, scripts and SVGs. No installation, framework, backend or build is required.

## Open and edit

Open `index.html` in a browser. Preserve the Arial/Helvetica body type, Georgia example heading and embedded portrait unless a change is approved. The editable copy and styling are outside the image's base64 data.

The 23 October revision continues the saved review implementation. Its flow is the paid-enrolment offer hero, four compact admissions-problem cards, a six-step approach with a compact differentiator and admissions diagram, founder context beside an illustrative qualification workflow, “Who It’s Not For” exclusions, the navy offer/guarantee panel with outcome and economics notes, native FAQs and a final invitation. The qualification workflow is an illustration, not client-results evidence. No testimonials, client counts or Canadian campaign outcomes are implied.

The main closing guidance is: “Reply to the message that brought you here. We will arrange a 20-minute call to review one course and decide whether this pilot is a sensible fit.” The page does not claim that clicking a button sends a reply.

The optional direct booking route retains the supplied Calendly destination:
`https://calendly.com/imhussain00112/free-growth-strategy-call`

There are four booking placements, all labelled “Arrange an intake review”: the shared desktop/mobile header link, hero, secondary link after the problem cards and final close. All four are ordinary links and work without JavaScript. JavaScript can update them from the `funnel-settings` JSON block. If changing the approved destination, update the static fallback links as well as `bookingUrl`. Invalid configuration cannot replace the approved fallback with an unsafe URL. No extra approach booking button is present.

## Navigation and motion

The header becomes sticky when JavaScript initialises it. “Your Challenges,” “My Approach,” “Who It’s Not For” and “FAQs” link to the actual revised sections. The exclusion link targets `#not-for`. The measured header height supplies the anchor offset; selected section links receive `aria-current="location"`. Native anchors and smooth scrolling are retained, with reduced-motion preferences respected.

At widths up to 960px, the same navigation and header booking link appear in a non-modal dropdown. The menu button exposes its expanded state, opening moves keyboard focus into the links, Escape closes it and restores button focus, and outside interaction or focus moving out dismisses it. Closed links are inert and hidden from assistive technology. Selecting a section closes the dropdown and focuses its heading. There is no modal role, scroll lock or focus trap. Without JavaScript, the menu toggle stays hidden and the navigation links remain visible inline.

Hero text, CTA and photograph have coordinated entrances while remaining immediately visible. Once-only section reveals use a short transform/fade, selected cards and approach steps stagger, and diagram nodes/connectors introduce their stages in sequence. The navy section's faint line texture moves through a slow 30-second cycle while it is in view. Its “Pause background motion” control pauses or resumes that effect; motion also pauses offscreen and when the document is hidden. Reduced motion disables these effects and hides the unnecessary ambient control. No animation library is used.

## Optional configuration

The `funnel-settings` block is near the end of the HTML:

| Setting | Behaviour |
| --- | --- |
| `bookingUrl` | Approved HTTPS destination shared by all booking links. |
| `founderPhoto` | Optional HTTPS or embedded JPEG/PNG/WebP/GIF override. A failed override restores the original portrait. |
| `videoEmbedUrl` | Approved Loom `/embed/ID`, YouTube privacy-mode `/embed/ID` or Vimeo `/video/ID` URL. The early video section stays hidden while missing or invalid. The iframe loads only after play; autoplay is removed. |
| `videoPoster` | Optional genuine approved poster. No poster is fabricated. |
| `videoTranscript` | Actual transcript only; use JSON-escaped newlines. |
| `canonicalUrl` | Final approved public page URL. |
| `readyForLaunch` | Keep `false` until the commercial terms, destination and publication are approved. Indexing is enabled only with this flag and valid booking/canonical URLs. It does not control visible internal labels; none are published. |

There are no external scripts, fonts, tracking pixels, calendar embeds or provider requests by default. The portrait is embedded. Motion progressively enhances visible content: hero entrances last 500ms with small offsets, section reveals use 500ms/14px movement, and diagram stages use 450ms entrances. Content is visible without JavaScript or IntersectionObserver; native FAQ disclosures, navigation and calendar links still work.

## Commercial review

The latest brief changes the draft offer from **30 unique qualified course enquiries** to **30 paid enrolments within 15 live advertising days** for one program assessed and agreed as suitable. The clock counts campaign running days after setup. This is a proposed commercial target, not a historical result or a promise that every enquiry converts. Earlier stages correctly continue to discuss enquiries and admissions conversations.

The draft defines an enrolment as a new student attributed to the agreed campaign, accepted into the selected program and paying the agreed course fee or qualifying deposit. It uses the requested full management-fee refund statement once under “My guarantee”. Attribution, payment and refund treatment still require written agreement; no executed terms document is implied.

Separate setup, advertising and software disclosures remain visible. Advertising budget is agreed separately and paid directly to Meta. Existing expense exclusions are preserved for review. Public numeric prices remain removed following the owner's 20 October instruction. The prior 30-live-day management period is recorded in the commercial decision list for confirmation under the changed offer; it is not silently replaced with a new duration.

The proposed payment trigger, ongoing free-work promise and 50-plus monthly claim remain outside public copy. “Zero financial risk” is removed. See the separate [commercial decisions](docs/COMMERCIAL-TERMS-2026-10-23.md) before publication.

The professional role line retains the user's wording: Meta Ads expert; Founder, Visionaryco / Visionaryskills; Digital marketing instructor. The user confirmed founding Visionary Skills on 20 October. These roles do not imply third-party certifications or Canadian campaign results.

See the [claim register](docs/CLAIMS.md) and [project/evidence/launch record](docs/PROJECT.md) for sources and review requirements. The 23 October brief supersedes older copy instructions and offer descriptions in dated records.

## Review and verification

The work remains on `review/funnel-design-refinements`, continuing the saved implementation. `main` is preserved. The current attachment is a text brief; no PDF comparison is claimed.

The 23 October revision passed 468 Chromium layout/behaviour checks at 13 widths from 320px to 1920px, plus 100 targeted checks after the final section-anchor adjustment and 133 rendered text-contrast checks. The final HTML and preceding full-suite hashes are distinguished in the [current verification record](docs/verification-revision-2026-10-23.json). Checks cover desktop/mobile navigation and sticky offsets, card alignment, native FAQs, all four intercepted Calendly routes, motion controls, reduced motion and no-JavaScript fallbacks. No overflow or JavaScript errors were found. No live appointment or calendar availability was tested. Firefox, Safari, real devices and a full automated accessibility scan were not tested.

Current actual browser renders: [desktop](docs/previews/2026-10-23/funnel-desktop.png), [mobile](docs/previews/2026-10-23/funnel-mobile.png), [problem cards](docs/previews/2026-10-23/problems-desktop.png), [mobile problem cards](docs/previews/2026-10-23/problems-mobile.png), [approach](docs/previews/2026-10-23/approach-desktop.png), [exclusions](docs/previews/2026-10-23/fit-mobile.png) and [offer](docs/previews/2026-10-23/offer-desktop.png). Section captures hide the sticky header only during capture; full-page images start at the top. The 22 October [verification record](docs/verification-navigation-2026-10-22.json), its 540 assertions and pre-existing files under `docs/previews/` describe the preceding implementation. They do not verify the revised paid-enrolment copy, six-step approach or exclusions. Automated accessibility checks do not provide a complete accessibility certification.

To save the standalone website from GitHub, open `index.html` on this review branch and select **Download raw file**. It includes its styles, scripts and portrait and needs no build.

No merge, deployment, Vercel protection change or indexing activation is authorised by this revision. For a separately authorised future static Vercel deployment, the existing settings remain: Other framework, repository root, no install/build command, output `.`. `readyForLaunch` stays false and robots remain `noindex, nofollow`. The supplied calendar destination is preserved; actual Calendly availability and duration are distinct from intercepted navigation tests. Actual Loom playback cannot be checked until a genuine URL is supplied.
