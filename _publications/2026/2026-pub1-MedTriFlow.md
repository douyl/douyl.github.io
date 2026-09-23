---
title:          "MedTriFlow: Efficient Resolution-Agnostic 3D Medical Image Generation with Implicit Triplane Representation"
date:           2026-06-01
selected:       false
pub:            "International Conference on Medical Image Computing and Computer Assisted Intervention (MICCAI)"
pub_date:       "2026"
abstract_short: >-
  3D medical image generation is crucial for data augmentation and downstream analysis but remains computationally expensive. We propose MedTriFlow, an efficient generative framework that bridges a discrete triplane latent space with a continuous anatomical field.
abstract_full: >-
  3D medical image generation is crucial for data augmentation and downstream analysis but remains computationally expensive. Existing voxel-based generative models operate on fixed-resolution grids, where the latent representation is coupled with output resolution. This leads to cubic scaling of computational costs and inability to generate volumes at varying resolutions without retraining. Triplane representations offer a more compact and efficient alternative. However, current triplane-based approaches either require costly instance-level optimization or are constrained by discrete voxel supervision, preventing resolution-agnostic generation. To address these challenges, we propose MedTriFlow, an efficient generative framework that bridges a discrete triplane latent space with a continuous anatomical field. The framework employs a triplane-based autoencoder with 3D-aware projection to compress volumetric data into a compact latent space, where generative modeling is performed for efficient generation. A continuous anatomical field, modeled by an implicit neural representation, then reconstructs volumetric anatomy at arbitrary resolutions, effectively enabling resolution-agnostic generation beyond the discrete voxel grid. Extensive experiments on diverse 3D datasets demonstrate that the proposed method, with fast inference (2.6s per volume at 256³) and resolution-agnostic generation (demonstrated up to 1024³), achieves superiority over recent 3D generative methods in generation quality, sparse-view CBCT and accelerated MRI reconstruction. Code and pre-trained models are available at https://github.com/ShanghaiTech-IMPACT/MedTriFlow.
cover:          /assets/images/covers/MedTriFlow.png
authors:
  - Chenfan Xu
  - Yulong Dou
  - Tao Luo
  - Qian Wang
  - Zhiming Cui
links:
  Code: https://github.com/ShanghaiTech-IMPACT/MedTriFlow
---
