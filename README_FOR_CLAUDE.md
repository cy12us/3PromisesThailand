# 3PromisesThailand — Seven-Page Design Handoff

**Prepared:** 2026-11-25  
**Scope:** Public-facing homepage plus six supporting pages. These are the user's approved **design prototypes**, **not a production deployment**.

## Working files

| File | Page / approved design |
|---|---|
| `index.html` | Homepage: deep teal/amber glow; four animated slides; State One regular rotation with optional manual click-to-crash; State Two three random automatic crashes total per four-slide cycle, plus optional manual crashes; scroll-synchronized falling words; six staggered bento cards; closing brand statement. |
| `three-promises.html` | Three Promises: muted sage background, subtle pastel panels, hover/tap-to-reveal wording, updated Promise Three stewardship of messages/special requests and provider arrangements. |
| `try-demo-free.html` | Demo doorway: **approved deep forest green** background; dashboard preview; explanation that entries cannot be saved; CTA to existing demo dashboard route. |
| `how-it-works.html` | **Latest approved design:** powder-blue background, four staggered hover/tap-to-expand bento steps, labels STEP ONE through STEP FOUR, Step Three explicitly mentions attachments, Day One pledge. |
| `pricing.html` | Warm-ivory Pricing: $49.99 to start, then $19.99/month for 36 months; no total price displayed; Day One pledge. |
| `contact.html` | Contact Us: sea-glass palette; info@3promisesthailand.com, Facebook, phone TBD, live chat coming soon. |
| `signup.html` | Sign Up Now: **approved soft pastel lavender** with shared glow; leads to the existing production waitlist until paid enrollment opens. |

All seven pages include local references to the **same** oak-emblem favicon assets (SVG/PNG/ICO), Apple touch icon, Android icons and `site.webmanifest`. Place these assets together in the same site root as the seven HTML pages.

## Navigation & currently incomplete destinations

- The six homepage bento cards are linked **locally** to their corresponding HTML pages in this package. All supporting pages return to `index.html`.
- `try-demo-free.html` links to `demo/dashboard.html`. **The real demo dashboard and its forms are NOT in this bundle**. Claude should connect the link to the separately developed demo files in the existing repository only after checking the actual route. Verify that demos cannot save/transmit any visitor input before launching.
- `signup.html` currently uses `https://www.3promisesthailand.com/#waitlist`, which points to the original waitlist. It is **not a working paid signup or checkout**. Preserve the existing waitlist and do not silently replace the destination with an unready paid enrollment.
- `contact.html` has working email and Facebook links. Phone and live chat are marked unavailable/coming soon; do not invent numbers, chat endpoints, or claim they work.
- These prototypes contain marketing statements about identity verification, record storage, and post-death stewardship. Their operational, privacy, legal, and technical requirements still require testing and review.

## Instructions for Claude

1. Verify you are working on the user's **`homepage-v2` development branch** of the existing repository (and that it is **not** the production branch) before changing tracked files. **Do not change `main` or deploy to production without explicit approval.**
2. Review each file against the existing repository structure. Preserve existing functional code and integrations that still need to be retained; especially the Supabase waitlist and authentication, Stripe integration, dashboard, and separate demo files.
3. Treat these seven files as the approved **public website visual baseline**. Avoid unrequested typography, color, wording, animation, or layout redesign.
4. Keep the new favicon assets together at the root, or adjust links to their deployed asset paths.
5. Connect the demo CTA only to the verified demo route; the sign-up CTA should continue to the waitlist until enrollment is operational.
6. Validate mobile behavior, keyboard access, hover/tap interactions, the four-slide timing, click-to-crash, the three automatic State Two crashes per round, and scroll synchronization.
7. Do **not** add backend writes to the demo. Avoid collecting customer data on these public design prototype pages.
8. Before publishing, review all statements and promises for actual service readiness, lawful release and notification rules, and accuracy.

## Source provenance

These are copies of the most recently approved designs in this ChatGPT conversation with two packaging-only changes:

1. Standardized the same local favicon links and assets across all seven pages.
2. Wired homepage bento buttons to their six corresponding public pages for local preview/testing. **No other visible design changes were intended.**

Original working source files are preserved outside this ZIP.
