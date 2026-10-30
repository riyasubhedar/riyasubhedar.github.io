# riyasubhedar.github.io

Source of my portfolio site, **https://riyasubhedar.github.io**: a PM in the AI era, learning and building, project by project.

Plain HTML and one stylesheet, hosted free on GitHub Pages. No build step.

## Adding a project

1. Copy `_template/case-study.html` to `projects/<slug>/index.html` and fill in every `{{…}}`.
2. Add screenshots to `assets/img/` as `<slug>-*.jpg` (about 1800 px wide).
3. Add a card under "Selected work" in `index.html`.
4. Preview locally: `python3 -m http.server 8000`, then open http://localhost:8000.

## Analytics

[GoatCounter](https://www.goatcounter.com): cookie-free and stores no personal data, so no consent banner. One script tag before `</body>` on every page (the code in `data-goatcounter` is the account's dashboard name). Outbound links carry `data-goatcounter-click="out-…"` names so clicks show up as events. Visits from localhost aren't counted; ad blockers hide some visitors, so numbers are a floor.

**Tagged links:** add `?campaign=<name>` (optionally `&ref=<source>`) to any link you share, e.g. `https://riyasubhedar.github.io/?campaign=<company>-<role>&ref=resume`. The campaign shows up in the dashboard's Campaigns panel when that link is opened. Keep the list of names you've used outside this public repo.

## Privacy guardrail

A pre-commit check (`scripts/check_private.py`, enabled with `git config core.hooksPath .githooks`) blocks email addresses, home-folder paths, API keys and the private terms listed in the never-committed `.private-terms` file.

© 2026 Riya Subhedar. All rights reserved.
