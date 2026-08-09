# julsoria.github.io

Personal academic homepage of **Jules Soria** — PhD candidate at CEA List, Université
Paris-Saclay, working on trustworthy AI: formal and interpretable explanations for AI systems.

Live at <https://julsoria.github.io/>.

Built with [Hugo Blox](https://hugoblox.com) (`academic-cv` template) and deployed to GitHub
Pages by GitHub Actions on every push to `main`.

## Where to edit what

| What | File |
|---|---|
| Name, bio, links, interests, education, experience, skills, languages | `data/authors/me.yaml` |
| Homepage sections (research blurb, publication lists, teaching) | `content/_index.md` |
| A publication | `content/publications/<slug>/index.md` |
| BibTeX source of truth | `publications.bib` (repo root) |
| Experience/CV page | `content/experience.md` |
| Site title, description, theme, math, analytics | `config/_default/params.yaml` |
| Site URL | `config/_default/hugo.yaml` |
| Navigation bar | `config/_default/menus.yaml` |
| Profile photo | `assets/media/authors/me.png` |

## Pending

- `assets/media/authors/me.png` is a **placeholder monogram** — drop in a real headshot at the
  same path (square, ideally ≥ 800×800). No other file needs changing.
- The **Download CV** button in `content/_index.md` is commented out. Uncomment it once a
  redacted CV — no phone number, no home address — is placed at `static/uploads/cv.pdf`.
- `content/publications/beyond-l2/` has no arXiv or Zenodo link yet; add them under
  `hugoblox.ids` once the preprint is posted.

## Local preview (optional)

CI builds on every push, so local tooling is not required. For a live-reload preview you need
Hugo Extended, Go (for Hugo Modules) and pnpm:

```bash
npm i -g hugo-extended@0.162.0
corepack enable pnpm && pnpm install
hugo server
```

## Deployment

`.github/workflows/deploy.yml` publishes via `actions/deploy-pages`. This requires
**Settings → Pages → Source = GitHub Actions** (one-time, in the repo settings).
