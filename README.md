# julsoria.github.io

Personal academic homepage of **Jules Soria** — PhD candidate at CEA List, Université Paris-Saclay, working on trustworthy AI: formal and interpretable explanations for AI systems.

Live at <https://julsoria.github.io/>.

Built with [Hugo Blox](https://hugoblox.com) (`academic-cv` template) and deployed to GitHub Pages by GitHub Actions on every push to `main`.

## Structure

Bilingual: English at the site root, French under `/fr/`. Five pages each, with no per-publication detail pages — publications link straight out to their own project pages.

| Page | English | French |
|---|---|---|
| About (bio, post-doc notice, news) | `content/en/_index.md` | `content/fr/_index.md` |
| Publications | `content/en/publications.md` | `content/fr/publications.md` |
| Talks / Exposés | `content/en/talks.md` | `content/fr/talks.md` |
| Teaching / Enseignement | `content/en/teaching.md` | `content/fr/teaching.md` |
| CV (experience, education, awards, service) | `content/en/cv.md` | `content/fr/cv.md` |

**Keep the two author profiles in step.** Hugo data files are not language-aware, so there are two: `data/authors/me.yaml` (used by the English pages via `username: me`) and `data/authors/me-fr.yaml` (French, `username: me-fr`). Any change to bio, role, education or experience must be mirrored in both, or the two languages will disagree.

| What else | Where |
|---|---|
| Languages, per-language menus and site description | `config/_default/languages.yaml` |
| Site title, theme (`mode: light`), math, spacing | `config/_default/params.yaml` |
| Site URL | `config/_default/hugo.yaml` |
| English navigation bar | `config/_default/menus.yaml` (French menu lives in `languages.yaml`) |
| Profile photo | `assets/media/authors/me.jpg` |
| Favicon | `assets/media/icon.png` — see below |
| Talk slides | `static/uploads/slides/` |
| Publication icons | inline emoji in the publications pages, matching each paper's project-page favicon (🍺 formal-ale, 📐 beyond-l2); YAGO uses `static/media/yago-mark.png` |

## Editing content

Entries are written as shortcodes, one call per entry, so there is no raw HTML to indent and no CSS in the content files. Each page carries a `HOW TO ADD …` block in its front matter with a copy-paste example.

| Shortcode | For | Example |
|---|---|---|
| `talk` | a talk | `{{< talk title="…" venue="Venue · City · Month Year" slides="2026-09-file.pdf" >}}` |
| `course` | a taught course or a supervision | `{{< course title="…" url="…" level="M2" where="Programme, Institution" >}}` |
| `svc` | an award, grant, organising or reviewing row | `{{< svc title="Top Reviewer" badge="NeurIPS 2026" note="…" >}}` |
| `pub` | a publication; paired, links written as markdown between the tags | `{{< pub icon="📐" title="…" authors="…" venue="…" >}}[arXiv](…)\n{{< /pub >}}` |
| `yr` | a year or group heading | `{{< yr title="2026" first="true" >}}` |
| `news` | a news item; paired, body written as markdown | `{{< news date="Oct 2026" star="true" >}}Awarded a **Top Reviewer** award.{{< /news >}}` |

They are defined in `layouts/_shortcodes/`, each with its parameters documented at the top of the file. `talk` translates its own link label (slides / diapositives) from the page language, so the two language versions stay identical apart from prose.

All the styling lives in one place, `layouts/_partials/hooks/head-end/entry-styles.html`. Change a rule there and it applies to every page in both languages.

**Every page exists twice.** A change to `content/en/<page>.md` must be mirrored in `content/fr/<page>.md`, and a change to `data/authors/me.yaml` in `data/authors/me-fr.yaml`.

## Theme overrides in `layouts/`

Two files shadow the upstream `HugoBlox/kit` `blox` module. Re-diff both against the module after any theme upgrade, and delete them if upstream fixes things.

- `_partials/functions/build_links.html` — **required to build at all.** Upstream initialises a Scratch key with `(dict)`, which yields a *nil* map, so the first `SetInMap` aborts the render with "assignment to entry in nil map". The stock template fails on any page with a `links:` block. One-line fix, commented in place.
- `_partials/hbx/blocks/markdown/block.html` — adds an opt-in `design.width: wide`. Upstream hardcodes `max-w-prose` + `lg:prose-xl`, far too narrow for a publication list with figures. Without the option the block renders exactly as upstream.

## Favicon

`assets/media/icon.png` only — deliberately **no** `icon.svg`. The theme's `get_site_icon` prefers an SVG and serves it from the fixed URL `/media/icon.svg`; browsers cache favicons hard and key that cache on the URL, so editing the file never reaches anyone who has already loaded the site. The PNG branch runs `.Fill`, which emits `/media/icon_hu_<hash>.png`, so every icon change busts its own cache. Note that an SVG would also leave the Apple touch icon resolving back to `media/icon.png`.

## Contact address

The e-mail address is never emitted at all. It appears only as the literal text `jules [dot] soria [at] cea [dot] fr`, styled as a monospace chip so it reads as an address to copy rather than a link. There is no `mailto:`, and no encoded copy of the address anywhere in the HTML — an earlier version stored it reversed in a `data-x` attribute and assembled the link in JavaScript, which is no longer needed.

The profile's envelope icon in both author profiles points at the `#postdoc` contact block, **not** a `mailto:`. Keep it that way: a plain link there would reintroduce the only harvestable copy of the address.

## Third-party assets

`static/media/yago-mark.png` is the emblem cropped from the YAGO project logo (<https://yago-knowledge.org/assets/images/logo.png>), used to identify the YAGO 4.5 paper. The YAGO site is licensed CC BY 4.0; the entry links back to yago-knowledge.org.

Talk slides in `static/uploads/slides/` are recompressed with `gs -dPDFSETTINGS=/ebook` (33 MB of originals down to 5.3 MB). Re-run that when adding a deck rather than committing the original.

## Pending

- **Profile photo**: `assets/media/authors/me.jpg`, 800×800, cropped square and centred on the face. To replace it, drop in a new square image at that path — the theme resolves the avatar as `media/authors/<username>.*`, so the French profile needs `me-fr.*` too, and `config/_default/module.yaml` mounts the one real file at that second path rather than keeping two copies. Change the extension there if the new file is not a `.jpg`. Hugo serves a content-hashed filename, so replacing the image busts its own cache. Note this is **not** the favicon, which comes from `assets/media/icon.png`.
- Clicking the photo plays one of five short animations, picked at random and never the same twice running (`layouts/_partials/hooks/head-end/avatar-interaction.html`). It is skipped entirely for anyone whose system asks for reduced motion.
- The **Download CV** button in the homepages is commented out. Uncomment it once a redacted CV — no phone number, no home address — is placed at `static/uploads/cv.pdf`.
- `content/en/talks.md` has a front-matter note listing two decks that could not be mapped to a venue.
- "Data Science" at CentraleSupélec has no course page, and its 2026 date is an assumption.

## Local preview (optional)

CI builds on every push, so local tooling is not required. For a live-reload preview you need Hugo Extended, Go (for Hugo Modules) and pnpm:

```bash
npm i -g hugo-extended@0.162.0
corepack enable pnpm && pnpm install
hugo server
```

Note: Tailwind's only source is `hugo_stats.json`, written by the previous build, and Hugo caches processed CSS under `resources/`. If a newly added utility class appears not to apply locally, `rm -rf resources public hugo_stats.json` and rebuild. Clean builds (what CI does) are always correct.

## Deployment

`.github/workflows/deploy.yml` publishes via `actions/deploy-pages`. This requires **Settings → Pages → Source = GitHub Actions** (one-time, in the repo settings).

Three workflows remain: `build.yml`, `deploy.yml`, and `upgrade.yml` (manual only).

Two upstream workflows were removed on purpose:

- **`import-publications.yml`** — it watched `publications.bib` and opened a PR generating one `content/publications/<slug>/index.md` page per entry. That is exactly the per-paper detail-page structure this site does not want, since each paper has its own project site. `publications.bib` is kept at the root as a citation reference only; nothing builds from it.
- **`internal-readme-news.yml`** — a bot that rewrote this README weekly with HugoBlox marketing.

`upgrade.yml` kept its manual trigger but lost its weekly cron, because an unattended theme upgrade would move the module out from under the two overrides in `layouts/`.
