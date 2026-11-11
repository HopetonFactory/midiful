# Midiful — support &amp; privacy pages

The public site for **Midiful** behind the two URLs Apple requires for App Store submission
(PF-PLAT-09). Static HTML, no build step, no trackers, no external requests.

| Page | URL |
|---|---|
| Support | https://hopetonfactory.github.io/midiful/ |
| Privacy Policy | https://hopetonfactory.github.io/midiful/privacy.html |

Issues on this repository are Midiful's support channel, so it must stay
**public** — a private repo would make the "Report a problem" link 404 for
everyone but the owner.

## Publishing

GitHub Pages, **Deploy from a branch** → `main` → `/ (root)`. No workflow needed.

## Editing

The source of truth is `site/` in the private `pianoflow` repository (the app's internal name); this repo is
the published copy. Change it there and copy across, so the pages cannot drift
from what the app actually does.

Keep the claims accurate — the support page states that Bluetooth MIDI is not
supported (PF-GAP-22) and that the app does not sound the piano part (PF-FR-07).
Revisit both whenever that changes.
