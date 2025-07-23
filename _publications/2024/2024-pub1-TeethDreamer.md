---
title:          "TeethDreamer: 3D Teeth Reconstruction from Five Intra-oral Photographs"
date:           2024-10-01
selected:       True
pub:            "International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI)"
pub_date:       "2024"
abstract_short: >-
  Orthodontic treatment usually requires regular face-to-face examinations to monitor dental conditions of the patients. When in person diagnosis is not feasible, an alternative is to utilize five intra-oral photographs for remote dental monitoring.
abstract_full: >-
  However, it lacks of 3D in formation, and how to reconstruct 3D dental models from such sparse view photographs is a challenging problem. In this study, we propose a 3D teeth reconstruction framework, named TeethDreamer, aiming to restore the shape and position of the upper and lower teeth. Given f ive intra-oral photographs, our approach first leverages a large diffu sion model’s prior knowledge to generate novel multi-view images with known poses to address sparse inputs and then reconstructs high-quality 3D teeth models by neural surface reconstruction. To ensure the 3D con sistency across generated views, we integrate a 3D-aware feature atten tion mechanism in the reverse diffusion process. Moreover, a geometry aware normal loss is incorporated into the teeth reconstruction process to enhance geometry accuracy. Extensive experiments demonstrate the superiority of our method over current state-of-the-arts, giving the po tential to monitor orthodontic treatment remotely.
cover:          /assets/images/covers/TeethDreamer.png
authors:
  - Chenfan Xu
  - Zhentao Liu
  - Yuan Liu
  - Yulong Dou
  - Jiamin Wu
  - Jiepeng Wang
  - Minjiao Wang
  - Dinggang Shen
  - Zhiming Cui
links:
  Project Page: https://shanghaitech-impact.github.io/TeethDreamer/
  Paper: https://papers.miccai.org/miccai-2024/paper/1038_paper.pdf
  Code: https://github.com/ShanghaiTech-IMPACT/TeethDreamer
---