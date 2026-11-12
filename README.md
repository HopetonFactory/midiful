# Midiful — support &amp; privacy pages

The public site for **Midiful** behind the two URLs Apple requires for App Store submission
(PF-PLAT-09). Static HTML, no build step, no trackers, no external requests.

| Page | URL | Used as |
|---|---|---|
| `index.html` | https://hopetonfactory.github.io/midiful/ | Marketing URL (optional) |
| `support.html` | https://hopetonfactory.github.io/midiful/support.html | **Support URL** (required) |
| `privacy.html` | https://hopetonfactory.github.io/midiful/privacy.html | **Privacy Policy URL** (required) |

Issues on this repository are Midiful's support channel, so it must stay
**public** — a private repo would make the "Report a problem" link 404 for
everyone but the owner.

## Publishing

GitHub Pages, **Deploy from a branch** → `main` → `/ (root)`. No workflow needed.

## Editing

The source of truth is `site/` in the private `pianoflow` repository (the app's internal name); this repo is
the published copy. Change it there and copy across, so the pages cannot drift
from what the app actually does.

Keep the claims accurate. The support page describes Bluetooth MIDI pairing,
which the app now does implement (REQ-TVM8 / PF-FR-41) — the older warning here
that it did not has been removed. It also states that the app does not sound the
piano part (PF-FR-07), which still holds. Revisit whenever either changes.
