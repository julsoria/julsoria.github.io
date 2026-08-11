---
title: 'CV'
date: 2026-08-09
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the author profile in `data/authors/`
#
# JDSE links to the stable Paris-Saclay landing page, NOT the dedicated conference site
# (hebergement.universite-paris-saclay.fr/jdse/jdse2026/), which returns nginx 502 as of
# 2026-08-11 in both curl and a browser. Swap the link back once that host is up again.
#
# Service record supplied by Jules (2026-08-11). Reviewer vs subreviewer follows his own
# labelling: he tagged ECAI 2025 and ECML PKDD 2026 as subreviews and left the rest untagged,
# so everything untagged is listed as reviewer. ACSAC 2025 is artifact evaluation, a distinct
# role. Correct here if WAISE 2024 or SAC 2025 were in fact subreviews.
#
# The `resume-skills` and `resume-languages` blocks were removed deliberately: they render
# self-rated proficiency as percentage bars and rings ("Python 100%", "Mandarin 20%"), which
# reads badly on an academic CV. The underlying `skills:` and `languages:` data is still in
# data/authors/me.yaml, so re-adding either block is a two-line change if ever wanted.

# Page sections
sections:
  - block: resume-experience
    content:
      username: me
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false

  - block: markdown
    id: service
    content:
      title: 'Service'
      text: |-
        <style>
        .entries .e{margin:0 0 1.4rem}
        .entries .t{font-weight:700;line-height:1.35;margin-bottom:.15rem}
        .entries .v{font-size:.94em;opacity:.85}
        .entries .badge{font-size:.78em;font-weight:600;letter-spacing:.02em;
          border:1px solid rgba(202,138,4,.55);color:#a16207;background:rgba(234,179,8,.12);
          border-radius:999px;padding:.05rem .5rem;margin-left:.35rem;white-space:nowrap}
        /* Use the theme's own `.dark` class. A `:root:not([data-theme=light])` selector would
           also match the default "system" state and put pale yellow on a white background. */
        .dark .entries .badge{color:#fde047}
        .entries h3{margin:0 0 1.25rem;padding-bottom:.35rem;
          border-bottom:1px solid rgba(120,120,120,.25)}
        .entries .grp{margin-top:2.25rem}
        </style>

        <div class="entries">

        <h3>Organizing</h3>

        <div class="e">
          <div class="t"><a href="https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering">Junior Conference on Data Science and Engineering (JDSE 2026)</a></div>
          <div class="v">Organizing committee &middot; 11th edition &middot; Université Paris-Saclay, Orsay &middot; 24–25 September 2026</div>
        </div>

        <h3 class="grp">Reviewing</h3>

        <div class="e">
          <div class="t">Reviewer</div>
          <div class="v">AAAI 2027 &middot; NeurIPS 2026 &middot; ICML 2026 <span class="badge">Gold Reviewer</span> &middot; AAAI 2026 &middot; SAC 2025 &middot; WAISE 2024</div>
        </div>

        <div class="e">
          <div class="t">Subreviewer</div>
          <div class="v">ECML PKDD 2026 &middot; ECAI 2025</div>
        </div>

        <div class="e">
          <div class="t">Artifact Evaluation Committee</div>
          <div class="v">ACSAC 2025</div>
        </div>

        </div>
    design:
      width: wide
      columns: '1'
---
