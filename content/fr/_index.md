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
        <div class="insts">
          <a href="https://list.cea.fr/en/" title="CEA List" style="--ar:1.99"><img class="lt" src="/media/inst/cea-list.svg" alt="CEA List"><img class="dk" src="/media/inst/cea-list-dark.svg" alt="CEA List"></a>
          <a href="https://www.universite-paris-saclay.fr/" title="Université Paris-Saclay" style="--ar:2.85"><img class="lt" src="/media/inst/paris-saclay.png" alt="Université Paris-Saclay"><img class="dk" src="/media/inst/paris-saclay-dark.png" alt="Université Paris-Saclay"></a>
        </div>

        <p class="rint">
          <strong>Thèmes de recherche</strong> &nbsp;·&nbsp; IA explicable formelle
          &nbsp;·&nbsp; Apprentissage interprétable &nbsp;·&nbsp; IA de confiance
        </p>
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: postdoc
    content:
      title: ''
      text: |-
        <div class="postdoc">
          <strong>Je recherche actuellement un post-doctorat.</strong>
          Je travaille sur l'explicabilité formelle et l'apprentissage automatique de confiance.
          Je serais heureux d'échanger avec des équipes travaillant sur les méthodes formelles
          pour l'apprentissage, l'interprétabilité ou la vérification de composants appris —
          <span class="eml">jules [dot] soria [at] cea [dot] fr</span>.
        </div>

        <hr class="sep">
    design:
      width: wide
      columns: '1'

  - block: markdown
    id: news
    content:
      title: 'Actualités'
      text: |-
        {{< news date="Oct. 2026" star="true" >}}
        Distinction **Top Reviewer** pour **NeurIPS 2026**.
        {{< /news >}}

        {{< news date="Oct. 2026" star="true" >}}
        Bourse **PACE** du CEA pour une visite de recherche dans un laboratoire européen.
        {{< /news >}}

        {{< news date="Sep. 2026" >}}
        Membre du comité d'organisation des [**11èmes JDSE**](https://www.universite-paris-saclay.fr/en/jdse-junior-conference-datascience-and-engineering), Université Paris-Saclay, 24–25 septembre.
        {{< /news >}}

        {{< news date="Sep. 2026" star="true" >}}
        Présentation de *Beyond $L_2$* à **ECML PKDD 2026**, Naples.
        {{< /news >}}

        {{< news date="Juil. 2026" star="true" >}}
        Distinction **<span class="gold">Gold</span> Reviewer** pour **ICML 2026**.
        {{< /news >}}

        {{< news date="Juil. 2026" >}}
        Exposé à **CAp & RFIAP 2026**, Montpellier.
        {{< /news >}}

        {{< news date="Juin 2026" >}}
        Exposé à l'atelier **NeuroSym4MLLM × EXPLAIN'AI**.
        {{< /news >}}

        {{< news date="Mai 2026" >}}
        Exposé au séminaire **NormaSTIC** sur l'explicabilité, Rouen · poster aux **CEA List Days**.
        {{< /news >}}

        {{< news date="Jan. 2026" >}}
        Présentation de *Formal Abductive Latent Explanations* à **AAAI 2026**, Singapour.
        {{< /news >}}

        {{< news date="Nov. 2025" star="true" >}}
        *Formal Abductive Latent Explanations* accepté à **AAAI 2026**.
        {{< /news >}}

        {{< news date="Oct. 2025" >}}
        Présentation de *Towards Abductive Latent Explanations* à **TRUST-AI @ ECAI 2025**, Bologne.
        {{< /news >}}

        {{< news date="Mars 2025" >}}
        Retour à Palaiseau après six mois au **National Institute of Informatics**, Tokyo.
        {{< /news >}}

        {{< news date="Sep. 2024" star="true" >}}
        Début d'un séjour de recherche dans l'équipe d'Isao Echizen au **NII Tokyo**, sur la robustesse adverse.
        {{< /news >}}

        {{< news date="Juil. 2024" >}}
        Présentation de *YAGO 4.5* à **SIGIR 2024**, Washington DC.
        {{< /news >}}

        {{< news date="Nov. 2023" star="true" >}}
        Début de ma thèse au **CEA List**, Université Paris-Saclay.
        {{< /news >}}
    design:
      width: wide
      columns: '1'
---
