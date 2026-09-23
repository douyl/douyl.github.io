---
title:          "OrthoFlow: Decoupled Landmark Prediction and Image Synthesis for Orthodontic Treatment Outcome Visualization"
date:           2026-06-02
selected:       true
pub:            "International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI)"
pub_date:       "2026"
abstract_short: >-
  Predicting post-treatment facial profiles from lateral cephalograms is clinically valuable for orthodontic planning and patient communication, yet remains challenging due to the complex interplay between skeletal, dental, and soft-tissue changes. We propose OrthoFlow, a two-stage decoupled generative framework that separates geometric prediction from image synthesis.
abstract_full: >-
  Predicting post-treatment facial profiles from lateral cephalograms is clinically valuable for orthodontic planning and patient communication, yet remains challenging due to the complex interplay between skeletal, dental, and soft-tissue changes. Conventional approaches either predict discrete clinical indices without visual output, or apply direct image-to-image translation that fails to preserve anatomical consistency. We propose OrthoFlow, a two-stage decoupled generative framework that separates geometric prediction from image synthesis. In the first stage, a Flow Matching model with a Graph-Transformer hybrid backbone predicts post-treatment landmark displacements conditioned on textual treatment plans. In the second stage, a conditional Flow Matching model synthesizes high-fidelity lateral cephalograms guided by the predicted anatomical contours. Experiments on a large-scale orthodontic dataset demonstrate that OrthoFlow achieves superior geometric accuracy and visual fidelity compared to existing methods, validated by both quantitative metrics and clinical evaluation by orthodontists. Our code and dataset are available at https://github.com/ShanghaiTech-IMPACT/OrthoFlow.
cover:          /assets/images/covers/OrthoFlow.png
authors:
  - Leyuan Wang*
  - Yulong Dou*
  - Jiancheng Yang
  - Guangying Song
  - Zhiming Cui
links:
  Code: https://github.com/ShanghaiTech-IMPACT/OrthoFlow
---
