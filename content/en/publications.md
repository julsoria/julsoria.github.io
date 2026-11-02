---
title: Publications
date: 2026-11-02
type: landing

design:
  spacing: '3rem'

# ─── HOW TO ADD A PUBLICATION ─────────────────────────────────────────────────────────
#   {{< pub icon="📐" title="Paper title"
#           authors="First Author, Second Author, …"
#           venue="Venue Year &middot; City, Country" >}}
#   [project page](https://…) [arXiv](https://…) [code](https://…)
#   {{< /pub >}}
#
#   The links between the tags are ordinary markdown — add or drop as many as you like.
#   icon   an emoji matching the paper's project-page favicon. Omit it to leave the column
#          empty; entries still line up.
#   img    use instead of icon for a logo, e.g. img="/media/yago-mark.png" alt="…".
#   type   "conference" or "workshop" — drives the filter buttons above the list.
#   core   CORE rank of the venue, shown as a badge: AAAI A*, ECML PKDD A, SIGIR A*.
#          Workshops have no CORE rank, so leave it off for those.
#   Year headings:  {{< yr title="2025" >}}   (add first="true" on the topmost one)
#   Keep publications.bib at the repo root in step; nothing builds from it, but it is the
#   citation reference. Mirror any change in content/fr/publications.md.
# ──────────────────────────────────────────────────────────────────────────────────────

sections:
  - block: markdown
    content:
      title: ''
      text: |-
        <div class="publist">

        Also on [Google Scholar](https://scholar.google.com/citations?user=1Qctec0AAAAJ) and [ORCID](https://orcid.org/0009-0009-6730-7406).

        {{< pubfilter >}}

        {{< yr title="2026" first="true" >}}

        {{< pub icon="📐" type="conference" core="A" title="Beyond $L_2$: Generalizing Abductive Latent Explanations to Diverse Prototype-Based Architectures"
                authors="Jules Soria, Alban Grastien, Romain Xu-Darme, Julien Girard-Satabin, Zakaria Chihani, Daniela Cancila"
                venue="ECML PKDD 2026, Research Track &middot; Naples, Italy" >}}
        [project page](https://beyond-l2.github.io/) [arXiv](https://arxiv.org/abs/2608.16773) [code](https://github.com/julsoria/beyond_l2) [models](https://zenodo.org/records/22311315)
        {{< /pub >}}

        {{< pub icon="🍺" type="conference" core="A*" title="Formal Abductive Latent Explanations for Prototype-Based Networks"
                authors="Jules Soria, Zakaria Chihani, Julien Girard-Satabin, Alban Grastien, Romain Xu-Darme, Daniela Cancila"
                venue="AAAI 2026, Main Technical Track &middot; Singapore" >}}
        [project page](https://formal-ale.github.io/) [arXiv](https://arxiv.org/abs/2511.16588) [code](https://github.com/julsoria/ale) [models](https://zenodo.org/records/16707325)
        {{< /pub >}}

        {{< yr title="2025" >}}

        {{< pub type="workshop" title="Towards Abductive Latent Explanations"
                authors="Jules Soria, Zakaria Chihani, Julien Girard-Satabin, Alban Grastien, Romain Xu-Darme, Daniela Cancila"
                venue="TRUST-AI workshop at ECAI 2025 &middot; Bologna, Italy &middot; CEUR-WS vol. 4132, 188–199" >}}
        [pdf](https://ceur-ws.org/Vol-4132/short34.pdf)
        {{< /pub >}}

        {{< yr title="2024" >}}

        {{< pub img="/media/yago-mark.png" alt="YAGO project logo" type="conference" core="A*"
                title="YAGO 4.5: A Large and Clean Knowledge Base with a Rich Taxonomy"
                authors="Fabian M. Suchanek, Mehwish Alam, Thomas Bonald, Lihu Chen, Pierre-Henri Paris, Jules Soria"
                venue="SIGIR 2024 &middot; Washington DC, USA &middot; 131–140" >}}
        [pdf](https://suchanek.name/work/publications/sigir-2024.pdf) [doi](https://doi.org/10.1145/3626772.3657876) [YAGO project](https://yago-knowledge.org/)
        {{< /pub >}}

        </div>
    design:
      width: wide
      columns: '1'
---
