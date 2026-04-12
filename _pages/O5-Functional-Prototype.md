---
layout: project
title: SLF – Initial Functional Prototype
permalink: /projects/slf/o5-functional-prototype/
description: Design and testing of a rotating mechanical system for guiding and capturing spotted lanternflies
technologies: [Mechanical Design, Prototyping, CAD, 3D Printing]

back_link: /projects/slf-2026/
back_text: Back to 2026 Project X-termination of SLF
---

# Project X-termination of SLF  
**Team:** SLF Crushers  

## Overview
This project explores the design and construction of an initial functional prototype aimed at capturing spotted lanternflies (SLF) through a passive mechanical guidance system. The goal was to develop a device that could reliably direct small objects (representing insects) into a contained chamber using only geometric constraints and rotational motion.

Rather than relying on active sensing or complex actuation, the system is built around a **purely mechanical approach**: guiding, funneling, and trapping through carefully designed geometry and controlled motion. This makes the design low-cost, scalable, and suitable for repeated outdoor use.

The prototype represents an early-stage validation of the concept, focusing on **mechanical feasibility, motion behavior, and reliability of transfer into the collection chamber**.

---

## System Architecture
The device is composed of several integrated subsystems that work together to achieve capture:

### Rotational Drive System
A low-speed DC motor (~3V, ~5 RPM) drives a D-profile shaft, which serves as the central axis of rotation. This shaft transmits torque to both the reaper wall and the rotating floor, ensuring synchronized motion across the system.

### Guidance Mechanism (Peg System)
The primary guiding mechanism consists of:
- A **peg plate** (stationary)
- A **reaper wall** with interlocking pegs (rotating)

As the reaper wall rotates, the interaction between the two peg arrays creates constrained pathways that push objects inward toward the center. This mechanism is designed to mimic a funneling effect without requiring continuous surfaces.

### Drop Mechanism
A **rotating floor** is attached to the same shaft. As it rotates, it periodically creates an opening aligned with the center of the system, allowing guided objects to fall into the chamber below.

### Collection Chamber
The **death chamber** serves as the final containment zone. Its geometry prevents escape and isolates captured objects from the active mechanical region.

Together, these subsystems create a sequential process:
1. Entry into the system  
2. Guidance toward the center  
3. Timed release via rotating floor  
4. Containment in chamber  

:contentReference[oaicite:0]{index=0}  

---

## Components and Fabrication
The prototype combines off-the-shelf components with custom-fabricated parts:

### Mechanical Components
- **D-profile rotary shaft** (carbon steel, 6 in, 0.25 in diameter)
- **DC motor** (3V, ~5 RPM)
- Shaft coupling and motor attachment interface

### Fabricated Components (PLA, 3D Printed)
- Reaper wall with integrated pegs  
- Peg plate (28 pegs)  
- Rotating floor  
- Motor attachment lid  
- Shaft connector  
- Collection chamber housing  

Most structural components were fabricated using PLA through rapid prototyping methods, enabling fast iteration and geometry adjustments. :contentReference[oaicite:1]{index=1}  

---

## Functional Behavior
During operation, the motor drives continuous rotation of the shaft. This produces two simultaneous effects:

- The **reaper wall rotates**, sweeping objects inward via peg interactions  
- The **rotating floor cycles**, intermittently opening a path to the chamber  

The design intentionally constrains motion so that objects cannot escape laterally. Side walls on the rotating floor further ensure that objects remain within the intended path until release.

This system relies heavily on:
- Geometric constraint  
- Friction interactions between objects and surfaces  
- Timing between rotation and drop alignment  

:contentReference[oaicite:2]{index=2}  

---

## Testing and Evaluation

### 1. Peg Guidance Test
**Objective:** Evaluate whether the peg mechanism successfully guides objects to the center  

**Method:**  
Crumpled paper balls were used as analogs for flies. These were placed at various entry positions, and the system was manually rotated.

**Results:**  
- Objects were consistently **crushed between pegs** rather than smoothly guided  
- Behavior was repeatable across multiple trials  

**Insight:**  
The peg geometry creates excessive compressive interaction instead of directional guidance.

**Next Iteration:**  
- Increase curvature of peg paths  
- Modify spacing to reduce pinching  
- Introduce smoother guiding surfaces  

---

### 2. Chamber Drop Test
**Objective:** Verify reliability of object transfer into the chamber  

**Method:**  
Objects were released near the center and observed during drop events.

**Results:**  
- 5/5 successful drops into chamber  
- No bounce-out or misalignment observed  

**Insight:**  
The drop mechanism is reliable, but throughput is limited.

**Next Iteration:**  
- Increase opening diameter  
- Add top cover to prevent escape  

---

### 3. Manual Rotation Test
**Objective:** Assess overall system behavior under continuous motion  

**Method:**  
The system was manually rotated for multiple full revolutions.

**Results:**  
- Rotation was possible but **not smooth**  
- Resistance occurred when pegs interacted  
- Entire device exhibited unwanted motion due to friction  

**Insight:**  
Mechanical tolerances and system stability are insufficient.

**Next Iteration:**  
- Add base weight for stability  
- Increase clearance between interacting components  
- Reduce friction points  

:contentReference[oaicite:3]{index=3}  

---

## Performance Criteria
The system was evaluated using the following criteria:

### Reliability of Transfer
Ability to consistently guide and deliver objects into the chamber without jamming.

### Smooth Mechanical Operation
Continuity of motion without excessive resistance or interruption.

### Structural Stability
Resistance to shaking, shifting, or unintended movement during operation.

### Efficiency
Speed and consistency of object transfer through the system.

A particularly important consideration for demonstration is **smooth motion**, as it directly reflects mechanical quality and reliability to observers. :contentReference[oaicite:4]{index=4}  

---

## Engineering Challenges 
This prototype revealed several key challenges:

- **Over-constrained geometry** causing jamming  
- **Friction-dominated interactions** reducing efficiency  
- **Tolerance sensitivity** in 3D printed parts  
- **System-level instability** due to unbalanced forces  

These challenges highlight the complexity of designing purely mechanical guidance systems at small scales.

---

## Reflection and Future Work
The prototype successfully validates the core concept of a rotational capture mechanism, demonstrating that passive geometry and motion can guide objects into a contained space.

However, it also reveals that **geometry design is critical**—small changes in spacing, curvature, and alignment significantly impact system behavior.

Future iterations will focus on:
- Redesigning peg geometry for smoother guidance  
- Reducing friction through material and tolerance adjustments  
- Improving system stability through mass distribution  
- Scaling the design for real-world insect interaction  

---

## Prototype
<img src="/assets/images/slf_prototype.png" alt="Prototype Image" width="400">