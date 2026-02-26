# MS-Human-700: Whole-body Human Musculoskeletal Model

<p align="center">
  <a href="https://lnsgroup.cc/research/MS-Human">Project page</a> | <a href="https://github.com/LNSGroup/msgym">Reinforcement Learning Environments (msgym)</a>
</p>


<div align="center">
  <img src="Pictures/ms_human_render_front.png" width="40%">
  <img src="Pictures/render_gif.gif" width="40%">
</div>

## Overview

This directory contains the **MuJoCo XML** and asset files for the **MS-Human-700** model.

Related papers:
- [MS-Human-700 (ICRA 2024)](https://arxiv.org/abs/2312.05473)
- [DynSyn (ICML 2024)](https://arxiv.org/abs/2407.11472)
- [MPC2 (ICLR 2025)](https://arxiv.org/abs/2505.08238)
- [QFlex (ICLR 2026)](https://arxiv.org/abs/2601.19707)

For reinforcement learning environments and training scripts, see [msgym](https://github.com/LNSGroup/msgym).

To visualize the models, drag-and-drop the `MS-Human-700-*.xml` files into MuJoCo's `simulate` viewer.

## Models

### Primary Model (Full Body)

**File:** `MS-Human-700.xml`

Full body human musculoskeletal model for whole-body locomotion tasks.

* **Bodies:** 90 (optimized to **80**)
* **Joints:** 206 (constrained to **85** for control stability)
* **Muscles:** 700 actuators

### Legs Locomotion Model

**File:** `MS-Human-700-Locomotion.xml`

Focusing on lower-body dynamics. This model isolates the legs for locomotion research while simplifying the upper limbs and torso.

* **Bodies:** 80
* **Joints:** 36
* **Muscles:** 100

### Unimanual Manipulation Model

**File:** `MS-Human-700-Manipulation.xml`

Focusing on right arm and detailed right hand, designed for manipulation tasks.

* **Bodies:** 127
* **Joints:** 42
* **Muscles:** 81

## Control Demo

[DynSyn](https://github.com/Beanpow/DynSyn) control results:

<div align="center">
  <img src="Pictures/loco_full_gif.gif" width="32%">
  <img src="Pictures/loco_legs_gif.gif" width="32%">
  <img src="Pictures/mani_gif.gif" width="32%">
</div>

[QFlex](https://lnsgroup.cc/research/Qflex) control results:

<div align="center">
  <img src="Pictures/run_gif.gif" width="49%">
  <img src="Pictures/dance_gif.gif" width="49%">
</div>