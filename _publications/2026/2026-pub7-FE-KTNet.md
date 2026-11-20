---
title:          "Cross-modality Knowledge Transfer Between fMRI and EEG for Improved Single-modality Alzheimer’s Disease Diagnosis"
date:           2026-11-18
selected:       false
pub:            "IEEE Transactions on Medical Imaging"
pub_date:       "2026"
abstract_short: >-
  Alzheimer’s disease (AD) involves complementary spatial and temporal brain changes that can be characterized by fMRI and EEG. We propose FE-KTNet, a three-stage framework that transfers knowledge learned from paired fMRI-EEG data to modality-specific models for single-modality diagnosis.
abstract_full: >-
  Alzheimer’s disease (AD) disrupts brain function in both spatial organization and temporal dynamics, which can be characterized by complementary fMRI and EEG measurements. In particular, fMRI provides higher spatial resolution to characterize multi-scale functional organization of brain networks, whereas EEG offers higher temporal resolution to capture dynamic neural activities across frequency bands. Thus, integrating the two modalities can characterize AD-related spatiotemporal disruptions more comprehensively than either modality alone. However, it is impractical to acquire paired fMRI and EEG data in real-world applications. To address this problem, we propose the fMRI-EEG Knowledge Transfer Network (FE-KTNet) to learn spatiotemporal representations from paired data and then transfer them back to modality-specific models through three stages. Specifically, in Stage 1, it learns modality-specific representations from fMRI and EEG FCNs, emphasizing multi-scale network organization for fMRI and frequency-specific electrophysiological coupling for EEG. Building on these representations, in Stage 2, it performs scale-wise bidirectional cross-modality fusion to integrate complementary information into fused multi-scale spatiotemporal representations. Finally, in Stage 3, it transfers the fused representations back to each modality-specific encoder through scale-wise feature alignment and logit-level knowledge distillation. We evaluate FE-KTNet on 14 multicenter datasets comprising 2,766 fMRI subjects and 1,842 EEG subjects, covering AD-NC, MCI-NC, and AD-MCI classifications. Compared with the corresponding baseline models, FE-KTNet increases fMRI-only and EEG-only accuracy by 3.4% and 6.1% for AD-NC classification, 5.2% and 8.0% for MCI-NC classification, and 3.5% and 7.1% for AD-MCI classification, respectively, and achieves the best overall performance among all evaluated methods. Our code is available at GitHub Repository.
cover:          /assets/images/covers/FE-KTNet.png
authors:
  - Xin Lin*
  - Yuxiao Liu*
  - Wenfei Yu*
  - Jiaxing Xu
  - Yulong Dou
  - Weiqi Li
  - Zhao Wu
  - Jiafan Qin
  - Xinyan Du
  - Jingjing Lin
  - Minhui Tan
  - Yuanzhe He
  - Feng Shi
  - Yansu Guo
  - Zhiming Cui#
  - Dinggang Shen#
links:
  Paper: https://ieeexplore.ieee.org/document/11803072
  Code: https://github.com/yizhixiaolinya/Code-TMI2026_fMRI-EEG
---
