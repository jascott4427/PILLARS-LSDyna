###### NOTE: Log files and notes are in markdown format meant for obsidian, but should work with other programs (https://obsidian.md/download)

# PILLARS-LSDyna: Plume-deployed Inflatable for Launch and Landing Abrasive Regolith Shielding

**Project Team:** Caltech PILLARS Team  
**Advisors:** Dr. Soon-Jo Chung (Caltech), Mr. Kalind Carpenter (JPL)  
**Lead Researcher (Deployment/Simulation):** James A. Scott III  

---

## Overview
This repository contains the **LS-DYNA** simulation framework for **PILLARS**, a toroidal membrane structure designed to mitigate lunar regolith ejecta damage during rocket landings. The simulation suite focuses on the structural dynamics of the shield under extreme conditions, including high-velocity plume impingement, thermal stresses, and regolith abrasion.

The project utilizes LS-DYNA's finite element analysis (FEA) capabilities to validate the shield's ability to maintain structural integrity while being hit by supersonic exhaust gases and abrasive particles.


---

## Features

* **Fluid-Structure Interaction (FSI):** Simulates the interaction between high-velocity rocket plumes and the flexible Kapton/Kevlar membrane.
* **Dynamic Deployment:** Models the skeletal bladder inflation sequence used for autonomous autonomous deployment.
* **Anchor Constraint Support:** Incorporates single-helix anchor node constraints to verify structural stability and stress distribution.
* **Lunar Environment Modeling:** Simulations configured for 1/6th Earth gravity and ambient lunar vacuum/temperature conditions.
* **Off-Nominal Case Testing:** Framework for testing "failure states," such as uneven inflation, anchor detachment, or off-center nozzle alignment.

---

## Simulation Architecture

The repository is structured to handle various stages of the FEA workflow:

* **Material Cards:** Custom definitions for Aluminized Kapton and Kevlar composites, including high-temperature performance parameters.
* **Nozzle Geometry:** Models for SpaceX Starship-class lander exhaust profiles to test plume velocity and temperature gradients.
* **Python Pre/Post-Processing:** Scripts to automate node merging, mesh refinement, and data extraction from LS-DYNA result files.
* **Obsidian Documentation:** Detailed technical logs and analysis notes formatted for easy viewing in Markdown.

---
