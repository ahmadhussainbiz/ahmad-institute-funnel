# Ahmad Institute Funnel

A complete five-section landing page for Ahmad Hussain, Founder of Visionary Co., and his course-enquiry pilot for independent Canadian training institutes.

## Open and edit

Open `index.html` in a browser. All CSS, JavaScript, page content, Ahmad's approved portrait and the text-based favicon are inside this file. No package installation, build process or backend is required.

The five sections are headline, what I do, who it is for, founder credibility, and the intake-review CTA. The same primary booking action appears in the hero and closing section, with no navigation menu or footer links. Native FAQ disclosures sit inside the final section.

The refined layout keeps the original Arial/Helvetica typography and Georgia working-principle quote. A white split hero, navy service section, light suitability section, near-black founder section and white closing section create purposeful contrast. On mobile, the offer and CTA precede a compact portrait. Motion is brief, adds no initial content hiding and respects reduced-motion preferences.

The latest review makes Ahmad's name the primary masthead identity, frames the original photograph in navy, increases smaller supporting text and polishes FAQ states. Card hover movement applies only to devices with a precise pointer. If an optional replacement photograph fails, the original embedded photograph is restored.

## Configure real links and assets

Find the `funnel-settings` JSON block near the end of `index.html`.

The supplied Calendly destination is now configured as `https://calendly.com/imhussain00112/free-growth-strategy-call`, enabling both booking buttons. It opens on activation rather than embedding or preloading a calendar. Loom is still missing and stays hidden. The page remains in design review with `readyForLaunch: false`.

Scroll entrances apply once to individual section introductions, service rows, suitability cards and closing content. They use a short 18px movement with a gentle fade and small paired-card delays. Content starts visible, no animation library is used, and reduced-motion preferences disable the effect.

| Setting | Use |
| --- | --- |
| `bookingUrl` | Approved HTTPS calendar destination. When empty or invalid, the booking button remains disabled with an honest scheduling message. |
| `founderPhoto` | Optional override for the approved portrait already embedded in the hero. Leave empty to keep the supplied photograph. Use an HTTPS image URL or a JPEG/PNG/WebP/GIF data URL. |
| `videoEmbedUrl` | Approved Loom `/embed/ID`, YouTube privacy-mode `/embed/ID`, or Vimeo `/video/ID` URL. The optional video block is hidden until configured. The iframe loads only after the viewer presses play. |
| `videoPoster` | Optional approved image for the video. |
| `videoTranscript` | Actual approved transcript. JSON requires escaped newlines as `\n`. No transcript is fabricated. |
| `canonicalUrl` | The final approved page URL. |
| `readyForLaunch` | Keep `false` until the booking URL, scope, budget periods and terms are approved. Setting this to `true` only removes the design-review label and changes indexing when valid booking and canonical URLs are also supplied. |

Use proper JSON quoting. Do not put tokens, passwords or personal student data in this file. All configured image/video providers are external requests; review the chosen assets and consent needs before activation. The default version loads no external scripts, fonts, images, calendars, trackers or videos.

`noindex` prevents deliberate indexing; it does not make a public URL private. Account-level deployment protection is separate.

## Offer wording

The target is 30 unique qualified enquiries in 15 live advertising days after campaign launch. Management covers 30 live advertising days. Setup, advertising and software costs are separate. The inconsistent 15–20-day sentence and internal future pricing stages are excluded.

Founder credibility is based on the supplied Pakistani advertising and teaching experience. No Canadian results, testimonials, student counts or approved client proof are invented.

The selected founder photo is now included. The reference set, video and proof assets remain open. Numerical client claims require confirmation of the number, wording and whether the experience belongs to Ahmad personally or Visionary Co. See `docs/PROJECT.md` for decisions, review notes and launch requirements.

## GitHub and Vercel

The review branch preserves `main` while the first version is reviewed. The website source is just `index.html`; this README and project notes are handover documentation.

For Vercel, import the GitHub repository and use a static/Other project with the repository root as the source directory and `.` as the output directory. No dependency installation or build command is needed. Current official build documentation confirms that Other serves the repository root when there is no `public` folder. Use a preview for review; production publication requires the real booking URL and final commercial terms.

## Verification

Static checks cover the five-section structure, consistent booking action, inline styles/scripts, link targets, heading hierarchy, configuration defaults, embedded portrait decoding, HTML parsing, JavaScript syntax and text contrast. Fourteen isolated behaviour checks cover both booking buttons, safe booking URLs, staging indexing, optional-media hiding, click-to-load video, optional image failures and reduced-motion/entry handling.

Actual browser inspection and any deployed preview are reported separately; source checks do not establish a conversion rate, complete accessibility certification or live booking delivery.

Before Calendly was supplied on 15 October 2026, Chromium validation passed 101 assertions covering responsive layouts at 11 widths from 320px to 1920px, keyboard interaction, JavaScript-disabled content, reduced motion, portrait fallback, URL handling and click-to-load video. Axe reported no automated WCAG A/AA violations at those widths. At that stage, booking and Loom links were missing. See the latest review record in `docs/PROJECT.md`. No merge or production deployment was performed.

After the Calendly and scroll update, 58 targeted Chromium assertions passed at 320, 390, 768, 1024 and 1440px. They cover both enabled buttons navigating to the exact supplied URL (intercepted), keyboard focus, one-time scroll activation, card hover after animation, reduced motion, no-JavaScript/no-IntersectionObserver fallbacks, portrait loading, unchanged offer terms and overflow. A direct request to Calendly was blocked by the environment proxy (CONNECT HTTP 403), so live event availability and duration were not verified and no appointment was made. Loom remains unconfigured. Fresh mobile and desktop screenshots were reviewed.
