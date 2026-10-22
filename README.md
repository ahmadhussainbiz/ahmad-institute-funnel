# Ahmad Institute Funnel

A founder-led course-enquiry funnel for Ahmad Hussain and independent Canadian training-provider owners and admissions decision-makers. The website is a single `index.html`, including the approved portrait, CSS, scripts and SVGs. No installation, framework, backend or build is required.

## Open and edit

Open `index.html` in a browser. Preserve the Arial/Helvetica body type, Georgia example heading and embedded portrait unless a change is approved. The editable copy and styling are outside the image's base64 data.

The page flows from the unchanged offer hero into four recognisable admissions problems, the feedback-based approach and diagram, editorial founder context beside an illustrative qualification workflow, a compact fit checklist, a navy offer/guarantee panel, neutral FAQs and a separate final booking invitation. The example is explicitly labelled as illustrative; it is not client-results evidence. No testimonials, client counts or Canadian campaign outcomes are implied.

All booking placements use the supplied Calendly destination:
`https://calendly.com/imhussain00112/free-growth-strategy-call`

There are four booking placements: the shared desktop/mobile header link, hero, secondary “Review my next intake” link after the problem cards, and final close. All four are ordinary links and work without JavaScript. JavaScript can update all of them from the `funnel-settings` JSON block. If changing the approved destination, update the static fallback links as well as `bookingUrl`. Invalid configuration cannot replace the approved fallback with an unsafe URL. No extra approach booking button is present.

## Navigation and motion

The professional header becomes sticky when JavaScript initialises it. “Your Challenges,” “My Approach,” “Who It’s For” and “FAQs” link to the real section headings. The measured header height supplies the anchor offset; selected section links receive `aria-current="location"`. Native anchor behaviour and smooth scrolling are retained, with reduced-motion preferences respected.

At widths up to 960px, the same navigation and header booking link appear in a non-modal dropdown. The menu button exposes its expanded state, opening moves keyboard focus into the links, Escape closes it and restores button focus, and outside interaction or focus moving out dismisses it. Closed links are inert and hidden from assistive technology. Selecting a section closes the dropdown and focuses its heading. There is no modal role, scroll lock or focus trap. Without JavaScript, the menu toggle stays hidden and the navigation links remain visible inline.

Hero text, CTA and photograph have coordinated entrances while remaining immediately visible. Once-only section reveals use a short transform/fade, selected cards and approach points stagger, and diagram nodes/connectors introduce their stages in sequence. The navy section's faint line texture moves through a slow 30-second cycle while it is in view. Its “Pause background motion” control pauses or resumes that ambient effect; motion also pauses offscreen and when the document is hidden. Reduced motion disables these effects and hides the unnecessary ambient control. No animation library is used.

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

## Commercial boundaries

The commitment is 30 unique qualified course enquiries in the agreed first 15 live advertising days after launch for one course and intake. Paid enrolments, applications and booked admissions meetings are distinct. Management covers 30 live advertising days.

Public pricing and the cost breakdown remain removed at the user's request on 20 October 2026; fees are discussed in the meeting. The conditional management-fee guarantee is retained verbatim without a numeric fee amount, with the existing exclusions and separate setup-failure remedy. Separate setup, advertising and software costs and the refund exclusions are plainly visible beside the offer, not only inside FAQs. No new commercial terms or future prices are invented. The word the user asked to remove remains absent from metadata, hidden-video labels and script-generated titles.

The main H1 is exactly “30 unique qualified course enquiries within 15 live advertising days.” The professional role line uses the user's supplied wording: Meta Ads expert; Founder, Visionaryco / Visionaryskills; Digital marketing instructor. The user explicitly confirmed founding Visionary Skills during this revision. These roles do not imply third-party certifications or Canadian campaign results.

See [claim register](docs/CLAIMS.md) and [project/evidence/launch record](docs/PROJECT.md) for sources, missing evidence and review requirements.

## Review and verification

The work is on `review/funnel-design-refinements`, based on the original `funnel-v1` HTML. `main` is preserved. The current request supplied a text brief, not a PDF or additional client assets, so no PDF comparison is claimed.

Actual Chromium screenshots: [desktop](docs/previews/desktop.png), [mobile](docs/previews/mobile.png), [qualification example](docs/previews/qualification-example.png). These show the rendered HTML, not a generated mockup. The project record lists the final browser checks and their limits. Automated accessibility checks are not a complete accessibility certification.

Header previews: [desktop](docs/previews/header-desktop.png), [mobile](docs/previews/header-mobile.png), [expanded mobile menu](docs/previews/menu-mobile.png). To save the standalone website from GitHub, open `index.html` on this review branch and select **Download raw file**. The file includes its styles, scripts and portrait and needs no build.

Section close-ups: [desktop problems](docs/previews/problems-desktop.png), [mobile problems](docs/previews/problems-mobile.png), [desktop approach](docs/previews/approach-desktop.png) and [mobile approach](docs/previews/approach-mobile.png). The navy section uses a tonal gradient, faint edge texture, lighter cards and outline icons without checkmarks. The diagram follows the three improvement points on a light approach surface; its aligned connectors and vertical mobile flow are retained. Distinct section surfaces replace repeated white-card wrappers.

The 22 October update passed **540 assertions** in Chromium: 470 main checks plus 70 independent supplemental checks. Eleven widths from 320px to 1920px cover desktop, tablet, mobile and both sides of the navigation breakpoint. Checks include anchors/offsets, active navigation during mouse-wheel scrolling, menu touch/keyboard/focus behaviour, all four intercepted booking destinations, native FAQs, one-time/staggered motion, ambient pause/resume, reduced motion, missing-observer and no-JavaScript fallbacks, preserved offer/fonts/portrait, no overflow and no measured hero layout shift. Automated WCAG A/AA scans reported zero violations, including open menus, expanded FAQs and first-frame text-contrast fixtures. See the [verification record](docs/verification-navigation-2026-10-22.json) for the tested HTML hash and current screenshot provenance. Firefox, Safari, real devices and native zoom were not tested; document visibility handling used simulated visibility events because headless Chromium kept both tabs visible.

No merge, production deployment, Vercel protection change or indexing activation is performed. For an eventual static Vercel deployment, the existing settings remain: Other framework, repository root, no install/build command, output `.`. Publication requires separate instruction. A direct Calendly check is blocked by the environment proxy; navigation can be tested without creating an appointment. Actual Loom playback remains untestable until a genuine URL is supplied.
