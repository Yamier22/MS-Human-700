# MS-Human-700: Whole-body Human Musculoskeletal Model

**Self model for embodied intelligence: Modeling full-body human musculoskeletal system and locomotion control with hierarchical low-dimensional representation (ICRA 2024)**

[**Project Page**](https://lnsgroup.cc/research/MS-Human) | [**Reinforcement Learning Environments (msgym)**](https://github.com/LNSGroup/msgym)


<div align="center">
  <img src="Pictures/ms_human_render_front.png" width="40%">
  <img src="Pictures/render_gif.gif" width="40%">
</div>

## Overview

This directory contains the **MuJoCo XML** and asset files for the **MS-Human-700** model. 

This model features a comprehensive musculoskeletal system ideal for embodied intelligence research. For reinforcement learning environments and training scripts, please refer to the **[msgym](https://github.com/LNSGroup/msgym)** repository.

To visualize the models, drag-and-drop the `MS-Human-700-*.xml` files into MuJoCo's `simulate` viewer.

## Models

### Primary Model (Full Body)

**File:** `MS-Human-700.xml`

Full body human musculoskeletal model with simplified hands and torso, for complex whole-body locomotion tasks.

*   **Bodies:** 90 (Optimized to **80**)
*   **Joints:** 206 (Constained to **85** for control stability)
*   **Muscles:** 700 actuators

<div align="center">
  <img src="Pictures/loco_full_gif.gif" width="60%">
</div>

### Legs Locomotion Model

**File:** `MS-Human-700-Locomotion.xml`

Focusing on lower-body dynamics. This model isolates the legs for locomotion research while simplifying the upper limbs and torso.

*   **Bodies:** 80
*   **Joints:** 36
*   **Muscles:** 100

<div align="center">
    <img src="Pictures/loco_legs_gif.gif" width="60%">
</div>

### Unimanual Manipulation Model

**File:** `MS-Human-700-Manipulation.xml`

Focusing on right arm and detailed right hand, designed for manipulation tasks.

*   **Bodies:** 127
*   **Joints:** 42
*   **Muscles:** 81

<div align="center">
    <img src="Pictures/mani_gif.gif" width="60%">
</div>