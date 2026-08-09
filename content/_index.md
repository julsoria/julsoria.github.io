---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-08-09
type: landing

sections:
  - block: resume-biography-3
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
      background:
        gradient_mesh:
          enable: false
      name:
        size: md # Options: xs, sm, md, lg (default), xl
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: markdown
    id: research
    content:
      title: '🔍 Research'
      subtitle: ''
      text: |-
        Machine learning models are increasingly deployed in settings where a wrong decision is
        expensive — and where "the model said so" is not an acceptable justification. My work sits
        at the intersection of **formal methods** and **explainable AI**, asking a deliberately
        narrow question: *when can an explanation be trusted?*

        Prototype-based, case-based reasoning networks (ProtoPNet and its descendants) are marketed
        as interpretable by design: each prediction comes with the prototypical training parts that
        supported it. But that guarantee is informal. Two inputs can receive an identical
        explanation and still be classified differently — so the explanation does not, on its own,
        account for the prediction.

        I develop **Abductive Latent Explanations (ALEs)**: sufficient conditions on a model's
        latent representation that *provably* imply its output. Computing them reduces to deriving
        tight bounds on latent-space distances, which makes them tractable without a SAT/SMT solver.
        Recent work generalises the framework beyond Euclidean latent spaces to the spherical,
        Gaussian and projection-based geometries used by modern architectures — enabling the first
        rigorous cross-architecture comparison of interpretability.

        I am always glad to discuss formal XAI, case-based reasoning, or trustworthy AI more
        broadly — feel free to [get in touch](mailto:jules.soria@cea.fr).
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: publications
    content:
      title: All Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  - block: markdown
    id: teaching
    content:
      title: '🎓 Teaching'
      subtitle: ''
      text: |-
        **2026**
        - *Information Systems and Programming (SIP)* — CentraleSupélec
        - *Advanced Deep Learning* — Master MVA
        - *Database Management Systems* — Université Paris Dauphine-PSL
        - *Computer Science Project* — ENSTA Paris

        **2025**
        - *Explainable & Trustworthy AI* — Université Grenoble Alpes

        **2024**
        - *Computer Science Project* — ENSTA Paris
    design:
      columns: '1'
---
