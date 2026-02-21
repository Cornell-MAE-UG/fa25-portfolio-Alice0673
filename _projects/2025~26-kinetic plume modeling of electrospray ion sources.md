---
layout: project
title: Kinetic Plume Modeling of Electrospray Ion Sources
permalink: /projects/slf-2026/
description: N-body simulation and defect sensitivity analysis for electrospray propulsion
technologies: [C++, Python, VTK, YAML, Numerical Simulation]
image: /assets/images/electrospray-plume.jpg
---

At the ASTRA Lab at Cornell University, I contribute to the development and validation of a kinetic N-body simulation framework used to model charged particle plume dynamics in electrospray propulsion systems.

Electrospray ion sources emit charged droplets and ions whose motion is governed by Coulomb interactions and space-charge effects. Accurately resolving plume evolution requires tracking many interacting particles over nanosecond timescales while preserving numerical stability and charge conservation.

This project focused on both **solver validation** and **geometric defect sensitivity analysis**, culminating in a peer-reviewed AIAA SciTech 2026 publication and Best Paper Award.

---

## Numerical Solver Development & Validation

I worked directly with the lab’s C++ N-body solver to ensure physical fidelity and computational robustness.

Key contributions included:

- Validating particle–particle Coulomb force calculations against analytic benchmarks  
- Performing timestep convergence studies to quantify numerical stability  
- Testing symmetry conditions and charge conservation under controlled configurations  
- Debugging particle injection and boundary handling modules  
- Managing structured YAML-based configuration files for reproducible parameter sweeps  

These validation efforts were essential to establish confidence in simulation results before performing large-scale parametric studies.

---

## Emitter–Extractor Defect Modeling

A central research question investigated how small geometric imperfections — specifically **emitter and extractor misalignment on the order of tens of microns** — influence plume behavior.

I contributed by:

- Modifying injection geometry within `particle_injection.cpp`  
- Parameterizing offset magnitudes through YAML configuration files  
- Generating controlled simulation datasets across multiple offset conditions  
- Quantifying plume divergence, radial spread, and species evolution  

Comparative simulations revealed measurable asymmetry in plume structure and shifts in particle-species distributions under increasing offset magnitudes, linking microscopic fabrication defects to macroscopic plume dynamics.

---

## Post-Processing & Visualization Pipeline

Raw simulation outputs are stored as `.vtp` (VTK PolyData) files containing particle trajectory and state data.

To enable systematic analysis, I developed a Python-based visualization and post-processing toolkit that:

- Parses and aggregates particle data across timesteps  
- Computes species-density histograms (neutrals through trimers)  
- Extracts time-of-flight distributions  
- Generates 3D trajectory visualizations  
- Automates figure production for batch simulation comparisons  

This pipeline significantly reduced manual processing time and enabled reproducible figure generation for publication.

---

## Results & Recognition

The findings from this work were published and presented at the **AIAA SciTech 2026 Forum**:

**Kinetic Plume Modeling of Electrospray Ion Sources With Emitter and Extractor Defects**  
AIAA-2026-2321

The paper received the:

**Best Paper Award — AIAA SciTech 2026**

This award recognizes outstanding technical contribution and analytical rigor among peer-reviewed conference submissions.

---

## Technical Skills Demonstrated

- N-body particle interaction modeling  
- Numerical stability and convergence analysis  
- Scientific C++ codebase modification  
- YAML-driven simulation parameter management  
- Python data analysis and VTK visualization  
- Publication-quality scientific figure generation  

---

This project integrates computational physics, propulsion modeling, and reproducible scientific workflow design to investigate defect-driven plume dynamics in electrospray systems.