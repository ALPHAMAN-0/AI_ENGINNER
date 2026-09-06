# AI_ENGINNER — CLAUDE.md

## Build / test / lint
- None found. No manifest (package.json/go.mod/pyproject.toml/Cargo.toml) exists in this repo.
- Run locally: `open index.html` (macOS) — or serve it: `python3 -m http.server 8000` (README.md).

## Rules observed
- Single self-contained file: all HTML/CSS/JS lives in `index.html`, "no dependencies" — don't split it into separate asset files without reason (README.md).
- Roadmap content is data: add/edit tasks via the `DATA` array in `index.html`, not by hand-writing markup (README.md "Editing the checklist").
- Task IDs are hashed from task text — editing an item's wording resets its saved checkbox state for users (README.md, index.html `hash()`).

## Read first
- `index.html` — the entire app (markup + CSS + JS)
- `README.md` — usage, deploy, and content-editing instructions
- `.github/workflows/deploy.yml` — GitHub Pages deploy trigger/steps

Architecture: see ARCHITECTURE.md — read before structural changes
