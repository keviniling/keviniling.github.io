---
layout: page
title: Distance-AF Multimer
description: Constraint-guided protein complex structure modeling with distributed multi-GPU optimization
img: 
importance: 2
category: research
---

## Distance-AF Multimer (Feb 2024 – Sept 2025)

**Role**: Lead Developer

A distributed multi-GPU optimization pipeline for protein-complex structure prediction that integrates user-supplied distance constraints with AlphaFold-Multimer, achieving up to ~60Å global-RMSD improvement on the hardest targets.

### Key Achievements

- Built a distributed multi-GPU optimization pipeline (PyTorch) for protein-complex structure prediction on 50k+ atom graphs
- Adapted the lab's Distance-AF method to complexes as a per-target, test-time optimization that fits user-supplied distance constraints with no retraining — robust to noisy and partial constraints
- Designed a coarse-to-fine, two-stage optimization that escapes local minima from AlphaFold-Multimer's poor initialization, eliminating flying residues and steric clashes
- Benchmarked across three datasets (27 hard multimeric targets, 8 peptide complexes, 3 large assemblies with 10+ chains); outperformed Chai-1, Protenix, and AlphaLink2 on Win/Tie/Loss

### Publications

- Ling, K. et al. "Peptide–protein docking: from physics-based models to generative intelligence." Chemical Communications, 2026
- Ling, K. et al. "Distance-AF Multimer: A Multi-Step Approach for Protein Complex Structure Modeling with User-Defined Distance Constraints." (In preparation)

### Technologies

- PyTorch, Distributed multi-GPU optimization
- AlphaFold2-Multimer integration
- Test-time optimization with experimental constraints

*Conducted at [Kihara Lab](https://kiharalab.org/), Purdue University*
