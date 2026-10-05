---
layout: page
title: NuFold Multimer
description: Generative modeling for RNA complexes with a Transformer and diffusion-based structure model
img: 
importance: 1
category: research
---

## NuFold Multimer (Jan 2026 – Present)

**Role**: Lead Developer

Generative modeling for RNA complexes: a Transformer-based RNA structure model extended from single-chain to multi-chain prediction, with a diffusion module that generates multiple candidate 3D structures.

### Key Contributions

- Extended a Transformer-based RNA structure model from single-chain to multi-chain prediction, integrating a diffusion module to generate multiple candidate 3D structures
- Built a data-curation and teacher-inference pipeline, running inference on approximately 20,000 RNA complexes; integrated multiple data sources, corrected inconsistent labels and identifiers, and applied confidence-based filtering for training
- Ran matched training ablations using 8 NVIDIA A100 80GB GPUs across 4 nodes to evaluate diffusion-decoder stability
- Enabled training crops of approximately 1,000 tokens by integrating NVIDIA cuEquivariance and a memory-efficient diffusion implementation
- Benchmarked AlphaFold3 and Boltz-2 on RNA complexes to compare prediction accuracy and characterize model limitations

### Technologies

- PyTorch, Transformers, Diffusion models
- Distributed multi-GPU training, GPU inference
- NVIDIA cuEquivariance
- Training with teacher-generated data

*Project ongoing at [Kihara Lab](https://kiharalab.org/), Purdue University*
