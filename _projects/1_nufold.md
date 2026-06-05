---
layout: page
title: NuFold Multimer
description: RNA-RNA complex structure prediction using diffusion-based deep learning
img: 
importance: 1
category: research
---

## NuFold Multimer (Jan 2026 – Present)

**Role**: Lead Developer

The first dedicated deep-learning predictor for RNA–RNA complexes, extending the lab's single-chain NuFold model to multi-chain inputs with a diffusion-based structure module and multi-sample conformational-ensemble generation.

### Key Contributions

- Extended the lab's single-chain NuFold model to multi-chain inputs with a diffusion-based structure module and multi-sample conformational-ensemble generation
- Built a large-scale model-distillation pipeline to overcome scarce ground truth: ran teacher-model inference (OpenFold3, Protenix) over ~20k RNA–RNA complexes with confidence-based filtering
- Curated a multi-source training set (RNAInter, RISE, snoDB) with tiered confidence stratification; debugged cross-database label errors to produce clean supervision
- Scaled training crops to ~1,000 tokens — beyond AlphaFold3's 768 — on substantially fewer GPUs by integrating NVIDIA cuEquivariance kernels and a memory-efficient diffusion module
- Benchmarked SOTA predictors (AlphaFold3, Boltz-2) on RNA–RNA complexes and showed none reliably handle them, establishing the need for a dedicated model

### Technologies

- PyTorch, Transformers, Diffusion models
- Distributed multi-GPU training/inference
- NVIDIA cuEquivariance GPU kernels
- Model distillation from OpenFold3, Protenix

*Project ongoing at [Kihara Lab](https://kiharalab.org/), Purdue University*
