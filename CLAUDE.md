# Working on this repo

Personal portfolio site for Nabil Arnaoot (n4bil.com). Plain static HTML on GitHub Pages, no build step; shared styles in `css/styles.css`, page-specific styles inline. See `README.md` for structure and design rules, and `plan/NEXT_SESSION.md` for the running handoff log.

## At the start of every session

Before anything else, remind Nabil of the **open items** listed at the top of `plan/NEXT_SESSION.md`. Keep it to a short list; then ask what he wants to work on.

## How we work

- Develop on the session's feature branch. When Nabil approves, open a PR to `master` and merge it with a **merge commit** (the repo's convention); GitHub Pages deploys from `master` in a minute or two.
- Before proposing a merge, check the change in headless Chromium: screenshots at 1280px and 390px, no horizontal overflow, and any `#anchor` links landing on their section. The sandbox usually can't reach the live site, so ask Nabil to hard-refresh when checking it.
- For bigger design changes, mock up first (screenshots) and let Nabil pick before building.
- Keep `README.md` and `plan/NEXT_SESSION.md` current as part of the work; remove assets the site no longer uses (they stay in git history — note the recovery commit).

## Design guardrails

The site was deliberately cleaned of AI-template tells (full list in `README.md` → "Design guardrails"). Don't reintroduce pill tags, chip rows, all-caps spaced labels, gradients, decorative shadows, identical pastel card grids, ghost numerals, or split title/intro page tops. KPIs are dashboard-style with a click-through to the right section. The painted Before/After illustrations stay.
