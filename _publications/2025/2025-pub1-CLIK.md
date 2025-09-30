---
title:          "CLIK-Diffusion: Clinical Knowledge-informed Diffusion Model for Tooth Alignment"
date:           2025-08-05
selected:       True
pub:            "Medical Image Analysis (MedIA)"
pub_date:       "2025"
abstract_short: >-
  Traditional semi-automatic methods for tooth alignment involve laborious manual procedures and heavily depend on the expertise of dentists, which often leads to inefficient and prolonged treatment durations.
abstract_full: >-
  Although many automatic methods have been proposed to assist especially the less experienced dentists, they often lack incorporating clinical insight and oversimplify the problem by estimating rigid transformation matrix for each tooth directly from dental point clouds.
  This over-simplification fails to capture nuanced requirements of orthodontic treatment, 
  i.e., specific clinical rules for effective alignment of misaligned teeth.
  To address this, we propose CLIK-Diffusion, a clinical knowledge-informed diffusion model for automatic tooth alignment.
  CLIK-Diffusion formulates the complex problem of tooth alignment as a more manageable landmark transformation problem, which is further refined into a landmark coordinate generation task.
  Specifically, we first detect landmarks for each tooth by category, and then build our CLIK-Diffusion to learn distribution of normal occlusion.
  To further encourage the integration of essential clinical knowledge, we design hierarchical constraints from three perspectives: 1) dental-arch level: to constrain arrangement of teeth from a global level; 2) inter-tooth level: to ensure tight contact and avoid unnecessary collision between neighboring teeth; and 3) individual-tooth level: to guarantee correct orientation of each tooth.
  In this way, our designed CLIK-Diffusion is able to predict the post-orthodontic landmarks that align with clinical knowledge, and then estimate rigid transformation for each tooth based on coordinates of its pre- and post-orthodontic landmarks.
  We have evaluated our CLIK-Diffusion on various malocclusion cases collected in real-world clinics, and demonstrate its exceptional performance and strong applicability in orthodontic treatment, compared with other state-of-the-art methods.
  The dataset and code will be released after acceptance of paper.
cover:          /assets/images/covers/CLIK-Diffusion.png
authors:
  - Yulong Dou
  - Han Wu
  - Changjian Li
  - Chen Wang
  - Tong Yang
  - Min Zhu
  - Dinggang Shen
  - Zhiming Cui
links:
  # Paper: https://authors.elsevier.com/a/1lYg74rfPmLfAq
  Paper: https://doi.org/10.1016/j.media.2025.103746
  Code: https://github.com/ShanghaiTech-IMPACT/CLIK-Diffusion
  Dataset: https://github.com/ShanghaiTech-IMPACT/CLIK-Diffusion/blob/main/Data_Access_Agreement.pdf
---