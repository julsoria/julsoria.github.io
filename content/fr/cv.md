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

        <h3>Distinctions</h3>

        <div class="e">
          <div class="t">Top Reviewer <span class="badge">NeurIPS 2026</span></div>
          <div class="v">Distinction attribuée aux relecteurs pour la qualité de leurs relectures</div>
        </div>

        <div class="e">
          <div class="t">Gold Reviewer <span class="badge">ICML 2026</span></div>
          <div class="v">Distinction attribuée aux relecteurs pour la qualité de leurs relectures</div>
        </div>

        <div class="e">
          <div class="t">Plan of Action for Cooperation in Europe (PACE) <span class="badge">CEA 2026</span></div>
          <div class="v">Bourse de mobilité du CEA, attribuée sur sélection, pour une visite de recherche courte dans un laboratoire européen &middot; 1 200 &euro;</div>
        </div>

        <h3 class="grp">Organisation</h3>

        <div class="e">
          <div class="t"><a href="https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering">Junior Conference on Data Science and Engineering (JDSE 2026)</a></div>
          <div class="v">Comité d'organisation &middot; 11ème édition &middot; Université Paris-Saclay, Orsay &middot; 24–25 septembre 2026</div>
        </div>

        <h3 class="grp">Financements</h3>

        <div class="e">
          <div class="t">SAIF — Safe Artificial Intelligence through Formal methods</div>
          <div class="v">Projet PEPR, France 2030 &middot; ANR-23-PEIA-0006 &middot; finance cette thèse</div>
        </div>

        <div class="e">
          <div class="t">Supercalculateur FactoryIA</div>
          <div class="v">Moyens de calcul pour les expériences, financés par le Conseil régional d'Île-de-France</div>
        </div>

        <h3 class="grp">Relecture</h3>

        <div class="e">
          <div class="t">Relecteur</div>
          <div class="v">AAAI 2027 &middot; NeurIPS 2026 &middot; ICML 2026 &middot; AAAI 2026 &middot; SAC 2025 &middot; WAISE 2024</div>
        </div>

        <div class="e">
          <div class="t">Sous-relecteur</div>
          <div class="v">ECML PKDD 2026 &middot; ECAI 2025</div>
        </div>

        <div class="e">
          <div class="t">Comité d'évaluation des artefacts</div>
          <div class="v">ACSAC 2025</div>
        </div>

        </div>
    design:
      width: wide
      columns: '1'
---
