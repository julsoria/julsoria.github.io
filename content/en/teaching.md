---
title: Teaching
date: 2026-11-02
type: landing

design:
  spacing: '3rem'

# ─── HOW TO ADD A COURSE ──────────────────────────────────────────────────────────────
#   {{< course title="Course name" url="https://syllabus-page" level="M2"
#              where="Programme, Institution" >}}
#
#   url    optional. Links the course title. Prefer the real syllabus page.
#   level  optional. Rendered as a pill: M2 / M1 / L3.
#   where  the institution line; may contain <a href="…">links</a>.
#   Year headings:  {{< yr title="2025" >}}   (add first="true" on the topmost one)
#   Mirror any change in content/fr/teaching.md.
#
# Course names come from each course's own page, which outranks the CSI slides: the MVA
# course is "Advanced Deep Learning" (formerly "Deep Learning in Practice").
# TODO (Jules): "Data Science" has no course page, and its 2026 date is an assumption.
# ──────────────────────────────────────────────────────────────────────────────────────

sections:
  - block: markdown
    content:
      title: ''
      text: |-
        <div class="entries">

        {{< yr title="2026" first="true" >}}

        {{< course logo="/media/inst/mva.png" title="Advanced Deep Learning" url="https://www.lri.fr/~gcharpia/dlip/" level="M2"
                   where="<a href=\"https://www.master-mva.com/\">Master MVA</a> and MSc AI, ENS Paris-Saclay" >}}

        {{< course logo="/media/inst/dauphine-psl.png" title="Database Management Systems" url="https://www.lamsade.dauphine.fr/~sworkman/dbms.html" level="M1"
                   where="Master IDD, LAMSADE — <a href=\"https://dauphine.psl.eu/\">Université Paris Dauphine-PSL</a>" >}}

        {{< course logo="/media/inst/centralesupelec.png" title="Systèmes d'Information et Programmation (SIP)" url="https://wdi.centralesupelec.fr/1CC1000/HomePage-Fr" level="L3"
                   where="1CC1000 — <a href=\"https://www.centralesupelec.fr/\">CentraleSupélec</a>" >}}

        {{< course logo="/media/inst/centralesupelec.png" title="Data Science" level="L3"
                   where="<a href=\"https://www.centralesupelec.fr/\">CentraleSupélec</a>" >}}

        {{< course logo="/media/inst/ensta.svg" title="Projet Informatique" url="https://synapses.ensta-paris.fr/catalogue/2025-2026/ue/16/CSC-3IN04-TA-projet-informatique" level="L3"
                   where="<a href=\"https://www.ensta-paris.fr/\">ENSTA Paris</a> — second year running" >}}

        {{< yr title="2025" >}}

        {{< course logo="/media/inst/uga.png" title="Explainable &amp; Trustworthy AI" url="https://m-ai.imag.fr/syllabus/cross-disc/explainable_trustworthy_ai/" level="M2"
                   where="Master of Artificial Intelligence, UFR IM²AG — <a href=\"https://www.univ-grenoble-alpes.fr/\">Université Grenoble Alpes</a>" >}}

        {{< yr title="2024" >}}

        {{< course logo="/media/inst/ensta.svg" title="Projet Informatique" url="https://synapses.ensta-paris.fr/catalogue/2025-2026/ue/16/CSC-3IN04-TA-projet-informatique" level="L3"
                   where="<a href=\"https://www.ensta-paris.fr/\">ENSTA Paris</a>" >}}

        {{< yr title="Supervision" >}}

        {{< course title="A. Peronnet — ProtoMelody" level="M1"
                   where="Co-supervised internship, CEA List" >}}

        </div>
    design:
      width: wide
      columns: '1'
---
