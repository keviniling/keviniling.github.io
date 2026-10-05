---
layout: page
title: Distance-AF Multimer
description: Constraint-guided protein complex modeling with per-target test-time optimization
img: 
importance: 2
category: research
---

## Distance-AF Multimer (Feb 2024 – Sept 2025)

**Role**: Lead Developer

Constraint-guided protein complex modeling: a per-target, test-time optimization that adapts pretrained model predictions to user-supplied geometric constraints without retraining, with up to 57.6 Å lower RMSD than AlphaFold-Multimer.

### Key Achievements

- Implemented per-target test-time optimization to adapt pretrained model predictions to user-supplied geometric constraints without retraining the underlying model
- Designed a coarse-to-fine optimization strategy to improve convergence from inaccurate initial predictions and reduce structural artifacts
- Built a PyTorch optimization workflow supporting structures with 50,000+ atoms, parallelizing independent target optimizations across GPUs
- Evaluated on 27 challenging multimer targets, 8 peptide complexes, and 6 assemblies with 5+ chains; achieved lower coordinate error (RMSD) than Chai-1, Protenix, and AlphaLink2 on 22/26, 19/27, and 26/27 benchmark targets, respectively
- Conducted ablations across 11 complexes with 0–30 distance constraints and uncertainty of ±2.5 Å and ±5 Å; retained acceptable docking accuracy on 8/11 targets under both uncertainty settings

### Publications

- Ling, K. et al. "Peptide–protein docking: from physics-based models to generative intelligence." Chemical Communications, 2026
- Ling, K. et al. "Distance-AF Multimer: A Multi-Step Approach for Protein Complex Structure Modeling with User-Defined Distance Constraints." (In preparation)

### Technologies

- PyTorch, multi-GPU optimization
- AlphaFold-Multimer integration
- Test-time optimization with user-supplied distance constraints

*Conducted at [Kihara Lab](https://kiharalab.org/), Purdue University*
