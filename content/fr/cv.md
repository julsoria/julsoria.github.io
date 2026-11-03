---
title: 'CV'
date: 2026-11-02
type: landing

design:
  spacing: '5rem'

# Version française de content/en/cv.md. Le bloc resume-experience lit le profil `me-fr`.
# Les blocs resume-skills et resume-languages sont volontairement absents : ils affichent
# des niveaux auto-évalués sous forme de barres et d'anneaux, ce qui passe mal sur un CV
# académique.

sections:
  - block: resume-experience
    content:
      username: me-fr
    design:
      date_format: 'January 2006'
      is_education_first: false

  - block: markdown
    id: service
    content:
      title: 'Distinctions et responsabilités'
      text: |-
        <div class="entries">

        {{< yr title="Distinctions" first="true" >}}

        {{< svc title="Top Reviewer" badge="NeurIPS 2026"
                note="Distinction attribuée aux relecteurs pour la qualité de leurs relectures" >}}

        {{< svc title=`<span class="gold">Gold</span> Reviewer` badge="ICML 2026"
                note="Distinction attribuée aux relecteurs pour la qualité de leurs relectures" >}}

        {{< svc title="Plan of Action for Cooperation in Europe (PACE)" badge="CEA 2026"
                note="Bourse de mobilité du CEA, attribuée sur sélection, pour une visite de recherche courte dans un laboratoire européen &middot; 1 200 &euro;" >}}

        {{< yr title="Organisation" >}}

        {{< svc title="Junior Conference on Data Science and Engineering (JDSE 2026)"
                url="https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering"
                note="Comité d'organisation &middot; 11ème édition &middot; Université Paris-Saclay, Orsay &middot; 24–25 septembre 2026" >}}

        {{< yr title="Financements" >}}

        {{< svc title="SAIF — Safe Artificial Intelligence through Formal methods"
                note="Projet PEPR, France 2030 &middot; ANR-23-PEIA-0006 &middot; finance cette thèse" >}}

        {{< svc title="Supercalculateur FactoryIA"
                note="Moyens de calcul pour les expériences, financés par le Conseil régional d'Île-de-France" >}}

        {{< yr title="Relecture" >}}

        {{< svc title="Relecteur"
                note="AAAI 2027 &middot; NeurIPS 2026 &middot; ICML 2026 &middot; AAAI 2026 &middot; SAC 2025 &middot; WAISE 2024" >}}

        {{< svc title="Sous-relecteur" note="ECML PKDD 2026 &middot; ECAI 2025" >}}

        {{< svc title="Comité d'évaluation des artefacts" note="ACSAC 2025" >}}

        </div>
    design:
      width: wide
      columns: '1'
---
