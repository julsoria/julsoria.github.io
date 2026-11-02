---
title: ''
summary: ''
date: 2026-11-02
type: landing

# Version française de content/en/_index.md. Les blocs pointent vers le profil `me-fr`
# (data/authors/me-fr.yaml) : les fichiers data ne sont pas multilingues.

sections:
  - block: resume-biography
    content:
      username: me-fr
      text: ''
      headings:
        about: ''
        education: ''
        interests: ''
    design:
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
          <strong>Thèmes de recherche</strong> &nbsp;·&nbsp; IA explicable formelle &nbsp;·&nbsp;
          Explications abductives &nbsp;·&nbsp; Réseaux à raisonnement par cas &nbsp;·&nbsp;
          Apprentissage interprétable &nbsp;·&nbsp; IA de confiance
        </p>
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: postdoc
    content:
      title: ''
      text: |-
        <style>
        /* Styled as a literal string, not a link: monospace and a faint chip so it reads
           unmistakably as an address to copy, with no hover/underline affordance. */
        .eml{font-family:ui-monospace,SFMono-Regular,"SF Mono",Menlo,Consolas,monospace;
          font-size:.92em;white-space:nowrap;background:rgba(120,120,120,.14);
          border-radius:5px;padding:.1rem .45rem}
        </style>

        <div style="border:1px solid rgba(37,99,235,.35);border-left:4px solid #2563eb;
          border-radius:10px;padding:1.1rem 1.4rem;background:rgba(37,99,235,.06)">
          <strong>Je recherche actuellement un post-doctorat.</strong>
          Je travaille sur l'explicabilité formelle et l'apprentissage automatique de confiance.
          Je serais heureux d'échanger avec des équipes travaillant sur les méthodes formelles
          pour l'apprentissage, l'interprétabilité ou la vérification de composants appris —
          <span class="eml">jules [dot] soria [at] cea [dot] fr</span>.
        </div>

    design:
      width: wide
      columns: '1'

  - block: markdown
    id: news
    content:
      title: 'Actualités'
      text: |-
        **Sep. 2026** — Membre du comité d'organisation des [**11èmes JDSE**](https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering), Université Paris-Saclay, 24–25 septembre.

        **Sep. 2026** — ⭐ Présentation de *Beyond $L_2$* à **ECML PKDD 2026**, Naples.

        **Août 2026** — *Beyond $L_2$* est désormais disponible en [prépublication sur arXiv](https://arxiv.org/abs/2608.16773).

        **Juil. 2026** — ⭐ Distinction **Gold Reviewer** pour **ICML 2026**.

        **Juil. 2026** — Exposé à **CAp & RFIAP 2026**, Montpellier.

        **Juin 2026** — Exposé à l'atelier **NeuroSym4MLLM × EXPLAIN'AI**.

        **Mai 2026** — Exposé au séminaire **NormaSTIC** sur l'explicabilité, Rouen · poster aux **CEA List Days**.

        **Jan. 2026** — ⭐ Présentation de *Formal Abductive Latent Explanations* à **AAAI 2026**, Singapour.

        **Nov. 2025** — ⭐ *Formal Abductive Latent Explanations* accepté à **AAAI 2026** ; [prépublication sur arXiv](https://arxiv.org/abs/2511.16588).

        **Oct. 2025** — Présentation de *Towards Abductive Latent Explanations* à **TRUST-AI @ ECAI 2025**, Bologne.

        **Mars 2025** — Retour à Palaiseau après six mois au **National Institute of Informatics**, Tokyo.

        **Sep. 2024** — ⭐ Début d'un séjour de recherche dans l'équipe d'Isao Echizen au **NII Tokyo**, sur la robustesse adverse.

        **Juil. 2024** — Présentation de *YAGO 4.5* à **SIGIR 2024**, Washington DC.

        **Nov. 2023** — ⭐ Début de ma thèse au **CEA List**, Université Paris-Saclay.
    design:
      width: wide
      columns: '1'
---
