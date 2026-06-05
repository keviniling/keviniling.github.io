---
layout: page
title: DAQ-Refine
description: Production web service for cryo-EM protein model refinement
img: 
importance: 3
category: research
related_publications: false
---

## DAQ-Refine (Aug 2023 – Jan 2024)

**Role**: Designer & Sole Developer

A production web service for cryo-EM protein model refinement, deployed as part of the published EMSuite server. Open-access and used by labs worldwide at ~10–20 jobs/month.

### Key Achievements

- Deployed the lab's cryo-EM refinement method as a production web service (React + Flask, Mol* 3D viewer)
- Re-architected from a usage-capped Colab notebook to a distributed backend, removing per-user limits and enabling large multimer jobs
- Runs and compares 3 refinement strategies and auto-selects the best result

### Technologies

- **Frontend**: React.js, Mol* 3D visualization
- **Backend**: Python, Flask, RESTful APIs
- **Infrastructure**: Distributed backend for large multimer jobs

### Live Demo

The tool is available at [em.kiharalab.org/algorithm/daq-refine](https://em.kiharalab.org/algorithm/daq-refine)

*Developed at [Kihara Lab](https://kiharalab.org/), Purdue University*
