---
title:          "COMET: Controllable Orthodontic Video Editing with Multi-view Estimation"
date:           2026-08-01
selected:       true
pub:            "Under Submission"
pub_date:       "2026"
abstract_short: >-
  Orthodontic treatment visualization is critical for patient decision-making and expectation management during lengthy and complex dental alignment procedures. We introduce COMET, a diffusion-based framework for controllable orthodontic video editing with multi-view estimation, which predicts structurally consistent post-treatment outcomes from pre-treatment videos and provides intuitive dynamic visualizations of expected results.
abstract_full: >-
  Orthodontic treatment visualization is critical for patient decision-making and expectation management during lengthy and complex dental alignment procedures. Existing methods predict static 2D images, and patients struggle to envision dynamic treatment outcomes from fixed-pose photographs alone. Two difficulties stand in the way of video-based prediction. First, paired pre- and post-treatment photographs are rarely available in real-world settings, so there is little direct supervision for learning orthodontic transformations. Second, the fine geometry of the teeth must stay consistent while head pose, viewpoint, and tooth visibility change from frame to frame. To address these difficulties, we introduce COMET, a diffusion-based framework for Controllable Orthodontic video editing with Multi-view EsTimation, which predicts structurally consistent post-treatment outcomes from pre-treatment videos and provides intuitive dynamic visualizations of expected results. COMET integrates an adapted ControlNet into a pretrained video diffusion model and augments it with two conditioning modules: (1) an Orthodontic Predictor that learns treatment-induced tooth movements from paired clinical 3D dental models and transforms the pre-treatment image in the first frame into a post-treatment image, and (2) a Multi-view Generator that estimates tooth contours across viewpoints so that the dental structures stay consistent across frames. In a user study with 18 participants, including three dentists, COMET receives the highest ratings on all criteria, and it improves tooth integrity from 0.74 to 0.87 over the best competing method on real-world videos. COMET provides a practical tool for offline orthodontic visualization and patient consultation.
cover:          /assets/images/covers/COMET.png
authors:
  - Lanzhuju Mei
  - Yulong Dou
  - Han Wu
  - Guo Chen
  - Zhiming Cui
  - Dinggang Shen
---
