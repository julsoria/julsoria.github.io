---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-08-09
type: landing

sections:
  # `resume-biography` (not `-3`) renders avatar, name, role, affiliation, links and bio
  # but NOT education — which lives on /cv/ instead. It also drops the interests list,
  # so that is re-added as the compact markdown block below.
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `data/authors/`)
      username: me
      text: ''
      # CV download button.
      # Uncomment once a redacted CV (no phone number, no home address) is placed at
      # `static/uploads/cv.pdf`.
      # button:
      #   text: Download CV
      #   url: uploads/cv.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Note: gradient_mesh renders a dark hero even in light mode, while this block's
      # text stays light-mode dark grey — unreadable. Leave it off.
      background:
        gradient_mesh:
          enable: false
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    id: interests
    content:
      title: ''
      text: |-
        <p style="text-align:center;opacity:.85">
          <strong>Research interests</strong> &nbsp;·&nbsp; Formal explainable AI &nbsp;·&nbsp;
          Abductive explanations &nbsp;·&nbsp; Case-based reasoning networks &nbsp;·&nbsp;
          Interpretable machine learning &nbsp;·&nbsp; Trustworthy AI
        </p>
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: postdoc
    content:
      title: ''
      text: |-
        <div style="border:1px solid rgba(37,99,235,.35);border-left:4px solid #2563eb;
          border-radius:10px;padding:1.1rem 1.4rem;background:rgba(37,99,235,.06)">
          <strong>I am currently looking for post-doc positions.</strong>
          I work on formal explainability and trustworthy machine learning. I would be glad to
          hear from groups working on formal methods for ML, interpretability, or the
          verification of learned components —
          <a href="mailto:jules.soria@cea.fr">jules.soria@cea.fr</a>.
        </div>
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: news
    content:
      title: 'News'
      text: |-
        **Sep 2026** — ⭐ *Beyond $L_2$* to be presented at **ECML PKDD 2026**, Naples.

        **Jul 2026** — Talk at **CAp & RFIAP 2026**, Montpellier.

        **Jun 2026** — Talk at the **NeuroSym4MLLM × EXPLAIN'AI** workshop.

        **May 2026** — Talk at the **NormaSTIC** seminar on explainability, Rouen · poster at **CEA List Days**.

        **Jan 2026** — ⭐ Presented *Formal Abductive Latent Explanations* at **AAAI 2026**, Singapore.

        **Nov 2025** — ⭐ *Formal Abductive Latent Explanations* accepted at **AAAI 2026**; [preprint on arXiv](https://arxiv.org/abs/2511.16588).

        **Oct 2025** — *Towards Abductive Latent Explanations* presented at **TRUST-AI @ ECAI 2025**, Bologna.

        **Mar 2025** — Back in Palaiseau after six months at the **National Institute of Informatics**, Tokyo.

        **Sep 2024** — ⭐ Started a research stay in Isao Echizen's lab at **NII Tokyo**, on adversarial robustness.

        **Jul 2024** — *YAGO 4.5* presented at **SIGIR 2024**, Washington DC.

        **Nov 2023** — ⭐ Started my PhD at **CEA List**, Université Paris-Saclay.
    design:
      width: wide
      columns: '1'
---
