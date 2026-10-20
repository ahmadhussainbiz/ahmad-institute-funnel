# Ahmad Institute Funnel

A founder-led course-enquiry funnel for Ahmad Hussain and independent Canadian training-provider owners and admissions decision-makers. The website is a single `index.html`, including the approved portrait, CSS, scripts and SVGs. No installation, framework, backend or build is required.

## Open and edit

Open `index.html` in a browser. Preserve the Arial/Helvetica body type, Georgia example heading and embedded portrait unless a change is approved. The editable copy and styling are outside the image's base64 data.

The page flows from the owner-focused hero through enquiry-to-admissions situations, an illustrative qualification workflow, a compact fit/founder section, and the commercial scope, FAQ and final call. The example is explicitly labelled as illustrative; it is not client-results evidence. No testimonials, client counts or Canadian campaign outcomes are implied.

All booking placements use the supplied Calendly destination:
`https://calendly.com/imhussain00112/free-growth-strategy-call`

There are exactly two booking links: the hero and final close. Both are ordinary links and work without JavaScript. JavaScript can update both from the `funnel-settings` JSON block. If changing the approved destination, update the static fallback links as well as `bookingUrl`. Invalid configuration cannot replace the approved fallback with an unsafe URL. No header or approach booking button is present.

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

There are no external scripts, fonts, tracking pixels, calendar embeds or provider requests by default. The portrait is embedded. Reveals progressively add a brief 300ms/8px entrance, play once and respect reduced motion. Content is visible without JavaScript or IntersectionObserver; native FAQ disclosures and calendar links still work.

## Commercial boundaries

The commitment is 30 unique qualified course enquiries in the agreed first 15 live advertising days after launch for one course and intake. Paid enrolments, applications and booked admissions meetings are distinct. Management covers 30 live advertising days.

Public pricing and the cost breakdown are removed at the user's request on 20 October 2026; fees are discussed in the meeting. The conditional management-fee guarantee is retained without a numeric fee amount, with the existing exclusions and separate setup-failure remedy. No new commercial terms or future prices are invented. The word the user asked to remove is also absent from metadata, hidden-video labels and script-generated titles.

The main H1 is exactly “30 unique qualified course enquiries within 15 live advertising days.” The professional role line uses the user's supplied wording: Meta Ads expert; Founder, Visionaryco / Visionaryskills; Digital marketing instructor. These are self-described roles, not third-party certifications or evidence of Canadian campaign results.

See [claim register](docs/CLAIMS.md) and [project/evidence/launch record](docs/PROJECT.md) for sources, missing evidence and review requirements.

## Review and verification

The work is on `review/funnel-design-refinements`, based on the original `funnel-v1` HTML. `main` is preserved. The current request supplied a text brief, not a PDF or additional client assets, so no PDF comparison is claimed.

Actual Chromium screenshots: [desktop](docs/previews/desktop.png), [mobile](docs/previews/mobile.png), [qualification example](docs/previews/qualification-example.png). These show the rendered HTML, not a generated mockup. The project record lists the final browser checks and their limits. Automated accessibility checks are not a complete accessibility certification.

Second-section close-ups: [desktop process](docs/previews/process-desktop.png) and [mobile process](docs/previews/process-mobile.png). The heading and outcome note are centred; the diagram retains aligned SVG connectors and a vertical mobile flow. The portrait uses layered CSS framing without modifying image bytes. The approach, fit/founder, commitment, FAQ and final-close sections share restrained outlines and geometric accents. The current version passed 302 browser assertions, including automated accessibility scans, at eleven widths; see the latest project record.

No merge, production deployment, Vercel protection change or indexing activation is performed. For an eventual static Vercel deployment, the existing settings remain: Other framework, repository root, no install/build command, output `.`. Publication requires separate instruction. A direct Calendly check is blocked by the environment proxy; navigation can be tested without creating an appointment. Actual Loom playback remains untestable until a genuine URL is supplied.
