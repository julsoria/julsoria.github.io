# julsoria.github.io

Personal academic homepage of **Jules Soria** — PhD candidate at CEA List, Université
Paris-Saclay, working on trustworthy AI: formal and interpretable explanations for AI systems.

Live at <https://julsoria.github.io/>.

Built with [Hugo Blox](https://hugoblox.com) (`academic-cv` template) and deployed to GitHub
Pages by GitHub Actions on every push to `main`.

## Structure

Five pages, no per-publication detail pages — publications link straight out to their own
project pages.

| Page | File |
|---|---|
| About (bio, post-doc notice, news) | `content/_index.md` |
| Publications | `content/publications.md` |
| Talks | `content/talks.md` |
| Teaching | `content/teaching.md` |
| CV (experience, education, skills, languages) | `content/cv.md` |

| What else | Where |
|---|---|
| Name, bio, links, interests, education, experience, skills, languages | `data/authors/me.yaml` |
| Site title, description, theme, math, spacing | `config/_default/params.yaml` |
| Site URL | `config/_default/hugo.yaml` |
| Navigation bar | `config/_default/menus.yaml` |
| Profile photo | `assets/media/authors/me.png` |
| Publication thumbnails | `static/media/` |

## Theme overrides in `layouts/`

Two files shadow the upstream `HugoBlox/kit` `blox` module. Re-diff both against the module
after any theme upgrade, and delete them if upstream fixes things.

- `_partials/functions/build_links.html` — **required to build at all.** Upstream initialises
  a Scratch key with `(dict)`, which yields a *nil* map, so the first `SetInMap` aborts the
  render with "assignment to entry in nil map". The stock template fails on any page with a
  `links:` block. One-line fix, commented in place.
- `_partials/hbx/blocks/markdown/block.html` — adds an opt-in `design.width: wide`. Upstream
  hardcodes `max-w-prose` + `lg:prose-xl`, far too narrow for a publication list with figures.
  Without the option the block renders exactly as upstream.

## Pending

- `assets/media/authors/me.png` is a **placeholder monogram** — drop in a real headshot at the
  same path (square, ideally ≥ 800×800). Nothing else needs changing.
- The **Download CV** button in `content/_index.md` is commented out. Uncomment it once a
  redacted CV — no phone number, no home address — is placed at `static/uploads/cv.pdf`.
- `content/talks.md` has a front-matter note listing three decks I could not map to a venue.
- Beyond-$L_2$ has no arXiv or Zenodo link yet; add to `content/publications.md` when posted.

## Local preview (optional)

CI builds on every push, so local tooling is not required. For a live-reload preview you need
Hugo Extended, Go (for Hugo Modules) and pnpm:

```bash
npm i -g hugo-extended@0.162.0
corepack enable pnpm && pnpm install
hugo server
```

Note: Tailwind's only source is `hugo_stats.json`, written by the previous build, and Hugo
caches processed CSS under `resources/`. If a newly added utility class appears not to apply
locally, `rm -rf resources public hugo_stats.json` and rebuild. Clean builds (what CI does)
are always correct.

## Deployment

`.github/workflows/deploy.yml` publishes via `actions/deploy-pages`. This requires
**Settings → Pages → Source = GitHub Actions** (one-time, in the repo settings).

Three workflows remain: `build.yml`, `deploy.yml`, and `upgrade.yml` (manual only).

Two upstream workflows were removed on purpose:

- **`import-publications.yml`** — it watched `publications.bib` and opened a PR generating
  one `content/publications/<slug>/index.md` page per entry. That is exactly the per-paper
  detail-page structure this site does not want, since each paper has its own project site.
  `publications.bib` is kept at the root as a citation reference only; nothing builds from it.
- **`internal-readme-news.yml`** — a bot that rewrote this README weekly with HugoBlox
  marketing.

`upgrade.yml` kept its manual trigger but lost its weekly cron, because an unattended theme
upgrade would move the module out from under the two overrides in `layouts/`.
