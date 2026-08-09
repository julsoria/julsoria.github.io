---
title: 'Beyond $L_2$: Generalizing Abductive Latent Explanations to Diverse Prototype-Based Architectures'

authors:
  - me
  - Alban Grastien
  - Romain Xu-Darme
  - Julien Girard-Satabin
  - Zakaria Chihani
  - Daniela Cancila

date: '2026-09-07T00:00:00Z'
publishDate: '2026-09-07T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: 'Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML PKDD), Naples, Italy'
  short_name: 'ECML PKDD 2026'

peer_reviewed: true

abstract: >-
  Prototype-based neural networks are hailed as interpretable-by-design architectures. Recently,
  Abductive Latent Explanations (ALE) were introduced to provide formal, mathematically
  guaranteed explanations that leverage the intrinsic structure of these networks to ensure both
  predictive safety and human readability. ALEs rely on computing tight bounds on latent space
  distances to produce formal explanations. However, existing ALE formulations are rigidly
  confined to Euclidean latent spaces. This leaves a critical gap: modern state-of-the-art
  architectures increasingly rely on non-Euclidean representations — spherical metrics, Gaussian
  densities, and dimensional projections — rendering current formal explanation methods
  incompatible. In this work, we generalize the ALE framework to support non-Euclidean prototype
  architectures. For each geometric variant, we systematically derive how to either map the
  architecture to existing bounds or construct novel, architecture-specific bounding algorithms.
  We validate our theoretical constructions by computing subset-minimal formal explanations on
  fully trained image classifiers. By unifying these diverse models under a single formal
  framework, we enable the first rigorous, cross-architecture comparison of their
  interpretability.

summary: >-
  Abductive Latent Explanations were confined to Euclidean latent spaces. We generalize them to
  spherical, Gaussian and projection-based prototype architectures, enabling the first rigorous
  cross-architecture comparison of interpretability.

tags:
  - Formal XAI
  - Interpretable Machine Learning
  - Abductive Explanations
  - Case-Based Reasoning

featured: true

links:
  - type: project
    url: https://beyond-l2.github.io/
    label: Project page
  - type: code
    url: https://github.com/julsoria/beyond_l2
---

To appear at ECML PKDD 2026, Naples, Italy, 7–11 September 2026.

This work was supported by the SAIF project, funded by "France 2030" (ANR-23-PEIA-0006), and
carried out using the FactoryIA supercomputer, financially supported by the Île-de-France
Regional Council.
