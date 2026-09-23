---
title:          "CMD-AD: Cross-Modality Distillation from fMRI-EEG for Single-Modality Alzheimer's Disease Diagnosis"
date:           2026-06-03
selected:       false
pub:            "International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI)"
pub_date:       "2026"
abstract_short: >-
  Alzheimer’s disease (AD) disrupts both the spatial organization and temporal dynamics of brain functional connectivity, which can be jointly characterized by fMRI and EEG. We propose CMD-AD (Cross-Modality Distillation for AD diagnosis), a three-stage framework that distills fused spatiotemporal knowledge into single-modality encoders to improve their performance.
abstract_full: >-
  Alzheimer’s disease (AD) disrupts both the spatial organization and temporal dynamics of brain functional connectivity, which can be jointly characterized by fMRI and EEG. fMRI-derived functional connectivity networks (FCNs) encode multiscale spatial topology, and EEG-derived FCNs capture multiband temporal coupling patterns, providing complementary information for AD diagnosis. However, paired fMRI-EEG acquisitions are rarely available in clinical practice, and existing fusion methods require both modalities at inference, limiting real-world deployment. To address this challenge, we propose CMD-AD (Cross-Modality Distillation for AD diagnosis), a three-stage framework that distills fused spatiotemporal knowledge into single-modality encoders to improve their performance. In Stage 1, hierarchical graph attention aggregation (HGAA) encoders are independently pretrained on each modality to extract multiscale fMRI spatial features and multiband EEG temporal features. In Stage 2, scale-wise bidirectional cross-modality fusion (BCMF) integrates fMRI and EEG representations at each parcellation scale, producing fused spatiotemporal targets. In Stage 3, teacher-student distillation transfers the fused spatiotemporal targets back to each modality-specific encoder, enabling accurate single-modality diagnostic performance without paired inputs. Evaluated on 8 multicenter datasets, CMD-AD improves fMRI-only accuracy from 73.51% to 75.50% and EEG-only accuracy from 63.52% to 65.02%, with AUC increasing from 80.88% to 83.70% and from 71.63% to 73.77%, respectively. These results demonstrate that cross-modality training can effectively enhance single-modality deployment for AD diagnosis. Our code is available at https://github.com/yizhixiaolinya/Code-MICCAI2026_fMRI-EEG.git.
cover:          /assets/images/covers/CMD-AD.png
authors:
  - Xin Lin*
  - Yuxiao Liu*
  - Wenfei Yu*
  - Yulong Dou
  - Weiqi Li
  - Minhui Tan
  - Yuanzhe He
  - Zhiming Cui#
  - Dinggang Shen#
links:
  Code: https://github.com/yizhixiaolinya/Code-MICCAI2026_fMRI-EEG
---
