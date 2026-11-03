---
title: 'CV'
date: 2026-08-09
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the author profile in `data/authors/`
#
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
      title: 'Awards & Service'
      text: |-
        <div class="entries">

        {{< yr title="Awards" first="true" >}}

        {{< svc title="Top Reviewer" badge="NeurIPS 2026"
                note="Awarded to reviewers recognised for the quality of their reviews" >}}

        {{< svc title=`<span class="gold">Gold</span> Reviewer` badge="ICML 2026"
                note="Awarded to reviewers recognised for the quality of their reviews" >}}

        {{< svc title="Plan of Action for Cooperation in Europe (PACE)" badge="CEA 2026"
                note="Competitive CEA mobility grant for a short research visit to an EU laboratory, awarded by a CEA selection committee &middot; &euro;1,200" >}}

        {{< yr title="Organizing" >}}

        {{< svc title="Junior Conference on Data Science and Engineering (JDSE 2026)"
                url="https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering"
                note="Organizing committee &middot; 11th edition &middot; Université Paris-Saclay, Orsay &middot; 24–25 September 2026" >}}

        {{< yr title="Funding" >}}

        {{< svc title="SAIF — Safe Artificial Intelligence through Formal methods"
                note="PEPR project, France 2030 &middot; ANR-23-PEIA-0006 &middot; supports this thesis" >}}

        {{< svc title="FactoryIA supercomputer"
                note="Compute for the experiments, financed by the Île-de-France Regional Council" >}}

        {{< yr title="Reviewing" >}}

        {{< svc title="Reviewer"
                note="AAAI 2027 &middot; NeurIPS 2026 &middot; ICML 2026 &middot; AAAI 2026 &middot; SAC 2025 &middot; WAISE 2024" >}}

        {{< svc title="Subreviewer" note="ECML PKDD 2026 &middot; ECAI 2025" >}}

        {{< svc title="Artifact Evaluation Committee" note="ACSAC 2025" >}}

        </div>
    design:
      width: wide
      columns: '1'
---
