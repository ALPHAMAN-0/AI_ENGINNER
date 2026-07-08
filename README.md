# AI Engineer — 2026 Roadmap Checklist

An interactive, self-tracking checklist for the 12–24 month path to becoming a
**frontier-lab generative AI engineer** — math → PyTorch → transformers/LLMs →
diffusion → GPU systems → original reproductions → career on-ramps.

- ✅ **4 phases**, **14 portfolio projects**, **~30 core papers**, plus resources & career checkpoints
- 💾 Progress is saved in your browser (localStorage) — no account, nothing sent anywhere
- 🔎 Search + filter by category (Math, Coding, LLMs, Diffusion, Systems, Projects, Papers, Career)
- 🌗 Light/dark theme, responsive, printable, with export/import of your progress
- 🔗 Every task links to the canonical free resource (Karpathy, CS336, arXiv, textbooks)

## View it locally

It's a single self-contained file — just open it:

```bash
open index.html          # macOS
# or serve it:
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy to GitHub Pages

This repo ships a GitHub Actions workflow ([`.github/workflows/deploy.yml`](.github/workflows/deploy.yml))
that publishes `index.html` on every push to `main`.

**One-time setup:**

1. Push this repo to GitHub (`main` branch).
2. Go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **GitHub Actions**.
4. Push to `main` (or run the workflow manually from the **Actions** tab → *Deploy to GitHub Pages* → *Run workflow*).

Your site goes live at:

```
https://<your-username>.github.io/<your-repo>/
```

For this repo that is: **https://alphaman-0.github.io/AI_ENGINNER/**

## Files

| File | Purpose |
| --- | --- |
| [`index.html`](index.html) | The entire interactive checklist (HTML + CSS + JS, no dependencies) |
| [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) | GitHub Pages deploy workflow |

## Editing the checklist

All tasks live in the `DATA` array inside `index.html`. Each item is:

```js
{ t: "Task text", cat: "llm", tag: "Project", links: [["Label", "https://…"]] }
```

`cat` sets the filter color; `tag` renders a small badge; `links` are optional.
Task IDs are hashed from the task text, so your saved progress survives reordering —
but **editing an item's text starts it fresh** as a new checkbox.

---

*Distilled from “The Complete 2026 Roadmap to Becoming a Frontier-Lab Generative AI Engineer.”
The field moves fast — verify resource availability before planning around it.*
