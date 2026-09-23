---
title:          "A Unified Latent Diffusion for High-Fidelity Any-to-Any Brain Modality Synthesis"
date:           2026-07-01
selected:       true
pub:            "6th Deep Generative Models Workshop at MICCAI (DGM4MICCAI)"
pub_date:       "2026"
pub_last:       "<strong><em style=\"color: rgb(192, 0, 0);\">(Long Oral)</em></strong>"
abstract_short: >-
  Comprehensive neurological diagnosis relies on the synergy of multimodal data from MRI, CT, and PET to capture distinct anatomical and pathological markers. To address incomplete imaging suites and the limitations of paired training data, we present BrainDiff, a unified latent diffusion framework for flexible any-to-any brain modality synthesis.
abstract_full: >-
  Comprehensive neurological diagnosis relies on the synergy of multimodal data from MRI, CT, and PET to capture distinct anatomical and pathological markers. However, clinical reality often results in incomplete imaging suites due to time constraint, high costs, or patient contraindication. Although cross-modality synthesis offers a potential solution, existing methods are limited by their reliance on strictly paired training data. This constraint prevents them from utilizing abundant single-modality data and from learning the distinct characteristics of each imaging domain, resulting in limited generative fidelity. To address these challenges, we present BrainDiff, a unified latent diffusion framework for flexible any-to-any brain modality synthesis. Our method employs a universal VQ-VAE to project all modalities into a shared latent space, where a prompt-guided diffusion model synthesizes corresponding images conditioned on descriptive prompts (e.g., patient attributes, imaging parameters). During cross-modality synthesis, a ControlNet module is incorporated to provide guidance that preserves anatomical structure of the source-modality image. Extensive multi-institutional experiments demonstrate that BrainDiff achieves state-of-the-art performance, delivering high-fidelity and anatomically consistent results for any-to-any generation. Code is available at https://github.com/douyl/BrainDiff.
cover:          /assets/images/covers/BrainDif.png
cover_style:    selected-cover-brain-diff
authors:
  - Yulong Dou*
  - Guo Chen*
  - Chenfan Xu
  - Yulin Wang
  - Zhe Xu
  - Zhiming Cui
  - Dinggang Shen
links:
  Code: https://github.com/douyl/BrainDiff
---
