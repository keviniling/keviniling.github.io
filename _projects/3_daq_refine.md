---
layout: page
title: DAQ-Refine
description: Public web service for cryo-EM protein model refinement
img: 
importance: 3
category: research
related_publications: false
---

## DAQ-Refine (Aug 2023 – Jan 2024)

**Role**: Designer & Sole Developer

A public web service for cryo-EM protein model refinement, integrated into the EMSuite server and used for approximately 10–20 refinement jobs per month.

### Key Achievements

- Independently built and deployed a public React/Flask application with interactive Mol* visualization
- Migrated a Colab workflow to lab infrastructure and automated SLURM job orchestration to run three refinement strategies per protein chain, select the best results, and assemble the final structure
- Developed reusable input-validation, early error-reporting, and progress-tracking components for integration with other EM-server algorithms
- Diagnosed recurring job failures reported by lab researchers and external users; added optional sequence alignment, specific input-error messages, and input-preparation documentation to help users resolve incompatible inputs

### Technologies

- **Frontend**: React.js, Mol* 3D visualization
- **Backend**: Python, Flask, REST APIs
- **Infrastructure**: SLURM job orchestration on lab infrastructure

### Live Demo

The tool is available at [em.kiharalab.org/algorithm/daq-refine](https://em.kiharalab.org/algorithm/daq-refine)

*Developed at [Kihara Lab](https://kiharalab.org/), Purdue University*
