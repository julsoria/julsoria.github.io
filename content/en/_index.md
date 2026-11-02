---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-08-09
type: landing

# Star convention: one star per paper, on its headline moment — the acceptance where
# there is one (AAAI), otherwise the presentation (ECML PKDD). Later appearances of the
# same paper stay plain, as do routine talks, so the stars mark distinct milestones.
#
# TODO (Jules): three award dates are placed, not sourced. Gold Reviewer sits at Jul 2026
# because that is when ICML 2026 ran (6–11 July, Seoul). The PACE grant is at Oct 2026
# because the dossier was finalised on 8 October, so the award must post-date that. The
# NeurIPS Top Reviewer month is a guess — no document for it was found on disk. Correct any
# of the three, and mirror the change in content/fr/_index.md.

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
        <div class="insts">
          <a href="https://list.cea.fr/en/" title="CEA List"><img src="/media/inst/cea-list.png" alt="CEA List"></a>
          <a href="https://www.universite-paris-saclay.fr/" title="Université Paris-Saclay"><img src="/media/inst/paris-saclay.png" alt="Université Paris-Saclay"></a>
        </div>

        <p style="text-align:center;opacity:.85">
          <strong>Research interests</strong> &nbsp;·&nbsp; Formal explainable AI
          &nbsp;·&nbsp; Interpretable machine learning &nbsp;·&nbsp; Trustworthy AI
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
          <span class="eml">jules [dot] soria [at] cea [dot] fr</span>.
        </div>

        <hr class="sep">
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: news
    content:
      title: 'News'
      text: |-
        {{< news date="Oct 2026" star="true" >}}
        Awarded a **Top Reviewer** award for **NeurIPS 2026**.
        {{< /news >}}

        {{< news date="Oct 2026" star="true" >}}
        Awarded a **CEA PACE** grant for a research visit to a European laboratory.
        {{< /news >}}

        {{< news date="Sep 2026" >}}
        Served on the organizing committee of the [**11th JDSE**](https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering), Université Paris-Saclay, 24–25 September.
        {{< /news >}}

        {{< news date="Sep 2026" star="true" >}}
        Presented *Beyond $L_2$* at **ECML PKDD 2026**, Naples.
        {{< /news >}}

        {{< news date="Jul 2026" star="true" >}}
        Awarded a **Gold Reviewer** badge for **ICML 2026**.
        {{< /news >}}

        {{< news date="Jul 2026" >}}
        Talk at **CAp & RFIAP 2026**, Montpellier.
        {{< /news >}}

        {{< news date="Jun 2026" >}}
        Talk at the **NeuroSym4MLLM × EXPLAIN'AI** workshop.
        {{< /news >}}

        {{< news date="May 2026" >}}
        Talk at the **NormaSTIC** seminar on explainability, Rouen · poster at **CEA List Days**.
        {{< /news >}}

        {{< news date="Jan 2026" >}}
        Presented *Formal Abductive Latent Explanations* at **AAAI 2026**, Singapore.
        {{< /news >}}

        {{< news date="Nov 2025" star="true" >}}
        *Formal Abductive Latent Explanations* accepted at **AAAI 2026**.
        {{< /news >}}

        {{< news date="Oct 2025" >}}
        *Towards Abductive Latent Explanations* presented at **TRUST-AI @ ECAI 2025**, Bologna.
        {{< /news >}}

        {{< news date="Mar 2025" >}}
        Back in Palaiseau after six months at the **National Institute of Informatics**, Tokyo.
        {{< /news >}}

        {{< news date="Sep 2024" star="true" >}}
        Started a research stay in Isao Echizen's lab at **NII Tokyo**, on adversarial robustness.
        {{< /news >}}

        {{< news date="Jul 2024" >}}
        *YAGO 4.5* presented at **SIGIR 2024**, Washington DC.
        {{< /news >}}

        {{< news date="Nov 2023" star="true" >}}
        Started my PhD at **CEA List**, Université Paris-Saclay.
        {{< /news >}}
    design:
      width: wide
      columns: '1'
---
