# Ahmad Institute Funnel

A complete five-section landing page for Ahmad Hussain, Founder of Visionary Co., and his course-enquiry pilot for independent Canadian training institutes.

## Open and edit

Open `index.html` in a browser. All CSS, JavaScript, page content and the text-based favicon are inside this file. No package installation, build process or backend is required.

The five sections are headline, what I do, who it is for, founder credibility, and the intake-review CTA. There is one primary booking button, no navigation menu and no footer links. Native FAQ disclosures sit inside the final section.

## Configure real links and assets

Find the `funnel-settings` JSON block near the end of `index.html`.

| Setting | Use |
| --- | --- |
| `bookingUrl` | Approved HTTPS calendar destination. When empty or invalid, the booking button remains disabled with an honest scheduling message. |
| `founderPhoto` | Ahmad's selected photo. Use an HTTPS image URL, or embed a JPEG/PNG/WebP/GIF data URL to retain a single-file deliverable. No old photo is selected automatically. |
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

The reference set, founder photo, video and proof assets remain open. See `docs/PROJECT.md` for decisions, review notes and launch requirements.

## GitHub and Vercel

The review branch preserves `main` while the first version is reviewed. The website source is just `index.html`; this README and project notes are handover documentation.

For Vercel, import the GitHub repository and use a static/Other project with the repository root as the source directory and `.` as the output directory. No dependency installation or build command is needed. Current official build documentation confirms that Other serves the repository root when there is no `public` folder. Use a preview for review; production publication requires the real booking URL and final commercial terms.

## Verification

Static checks cover the five-section structure, one booking action, inline styles/scripts, link targets, heading hierarchy, configuration defaults, HTML parsing and JavaScript syntax. Behaviour checks cover safe booking URLs, staging indexing, optional-media hiding, click-to-load video and optional image failures.

Actual browser inspection and any deployed preview are reported separately; source checks do not establish a conversion rate, complete accessibility certification or live booking delivery.
