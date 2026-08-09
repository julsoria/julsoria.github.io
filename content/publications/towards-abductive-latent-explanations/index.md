---
title: 'Towards Abductive Latent Explanations'

authors:
  - me
  - Zakaria Chihani
  - Julien Girard-Satabin
  - Alban Grastien
  - Romain Xu-Darme
  - Daniela Cancila

date: '2025-10-25T00:00:00Z'
publishDate: '2025-10-25T00:00:00Z'

publication_types: ['paper-conference']

publication:
  name: 'European Workshop on Trustworthy AI (TRUST-AI) at ECAI, CEUR Workshop Proceedings, Vol. 4132, 188–199'
  short_name: 'TRUST-AI @ ECAI 2025'

peer_reviewed: true

abstract: >-
  Case-based reasoning networks are machine-learning models that make predictions based on
  similarity between the input and prototypical parts of training samples, called prototypes.
  Such models are able to explain each decision by pointing to the prototypes that contributed
  the most to the final outcome. As the explanation is a core part of the prediction, they are
  often qualified as "interpretable by design". While promising, we show that such explanations
  are sometimes misleading, which hampers their usefulness in safety-critical contexts. In
  particular, several instances may lead to different predictions and yet have the same
  explanation. Drawing inspiration from the field of formal eXplainable AI (formal XAI), we
  propose Abductive Latent Explanations (ALEs), a formalism to express sufficient conditions on
  the intermediate (latent) representation of the instance that imply the prediction. Our
  approach combines the inherent interpretability of case-based reasoning models and the
  guarantees provided by formal XAI. We propose a solver-free and scalable algorithm for
  generating ALEs and present the feasibility of our approach on the CUB-200 dataset for the
  task of fine-grained image classification.

summary: >-
  The workshop paper that introduced Abductive Latent Explanations, with a first feasibility
  study on CUB-200 fine-grained image classification.

tags:
  - Formal XAI
  - Case-Based Reasoning
  - Trustworthy AI

featured: false
---

Workshop version, later extended into the AAAI 2026 paper
[*Formal Abductive Latent Explanations for Prototype-Based Networks*](/publications/formal-abductive-latent-explanations/).
