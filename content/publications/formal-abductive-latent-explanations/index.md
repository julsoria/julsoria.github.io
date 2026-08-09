---
title: 'Formal Abductive Latent Explanations for Prototype-Based Networks'

authors:
  - me
  - Zakaria Chihani
  - Julien Girard-Satabin
  - Alban Grastien
  - Romain Xu-Darme
  - Daniela Cancila

date: '2026-01-20T00:00:00Z'
publishDate: '2026-01-20T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: 'Proceedings of the AAAI Conference on Artificial Intelligence, 40(30), 25590–25598'
  short_name: 'AAAI 2026'

peer_reviewed: true

abstract: >-
  Case-based reasoning networks are machine-learning models that make predictions based on
  similarity between the input and prototypical parts of training samples, called prototypes.
  Such models are able to explain each decision by pointing to the prototypes that contributed
  the most to the final outcome. As the explanation is a core part of the prediction, they are
  often qualified as "interpretable by design". While promising, we show that such explanations
  are sometimes misleading, which hampers their usefulness in safety-critical contexts. In
  particular, several instances may lead to different predictions and yet have the same
  explanation. Drawing inspiration from the field of formal eXplainable AI (FXAI), we propose
  Abductive Latent Explanations (ALEs), a formalism to express sufficient conditions on the
  intermediate (latent) representation of the instance that imply the prediction. Our approach
  combines the inherent interpretability of case-based reasoning models and the guarantees
  provided by formal XAI. We propose a solver-free and scalable algorithm for generating ALEs
  based on three distinct paradigms, compare them, and present the feasibility of our approach
  on diverse datasets for both standard and fine-grained image classification.

summary: >-
  Explanations from prototype-based networks can be misleading. We introduce Abductive Latent
  Explanations — sufficient conditions on the latent representation that provably imply the
  prediction — and a solver-free algorithm to compute them.

tags:
  - Formal XAI
  - Prototype-Based Networks
  - Abductive Explanations

featured: true

hugoblox:
  ids:
    arxiv: '2511.16588'
    zenodo: '16707325'

links:
  - type: project
    url: https://formal-ale.github.io/
    label: Project page
  - type: code
    url: https://github.com/julsoria/ale
---

Presented in the AAAI 2026 Main Technical Track.

This work was supported by the SAIF project, funded by "France 2030" (ANR-23-PEIA-0006), and
carried out using the FactoryIA supercomputer, financially supported by the Île-de-France
Regional Council.
