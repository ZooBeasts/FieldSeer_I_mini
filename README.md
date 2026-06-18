
 # FieldSeer-Mini: A Minimal World Model for FDTD Sequence Prediction

> **Disclaimer**: This is a minimal, open-source educational baseline implementation of the core idea behind **FieldSeer I** (Guo, 2025). It demonstrates the feasibility of using world models to predict spatiotemporal field evolution in 2D FDTD simulations. This version is intentionally simplified and does not include the full suite of physics-guided components, geometry-aware conditioning, or online adaptation mechanisms described in the paper — those are reserved for proprietary and patent-pending systems.


<img width="1000" height="320" alt="epoch_0180_rollout_sequence" src="https://github.com/user-attachments/assets/5d2d734f-175a-4b77-9481-56e02de0be38" />

## What it does
- Generates synthetic 2D FDTD waveguide data with circular inclusions.
- Trains a GRU world model to predict future field frames from a prefix.
- Visualizes real vs. predicted field evolution via animated GIFs.

## What it doesn't do (yet)
- Handle multi-material or complex geometries (no GNN encoder).
- Guarantee long-horizon physical stability (no symlog/symexp or physics-based regularization).
- Support real-time geometry editing or online adaptation.
- Evaluate optical responses (R/T/A) — only pixel-level MSE is reported.

## Purpose
This repository serves as:
1. A **proof-of-concept** for applying world models to computational electromagnetics.
2. An **open benchmark** for the community to build upon.
3. A **minimal baseline** for comparison with future work.

For the full, production-grade system with physics-guided stability and geometry-aware control, please refer to the publications:  
**FieldSeer I: FieldSeer I: Physics-Guided World Models for Long-Horizon Electromagnetic Dynamics under Partial Observability**.
<img width="3375" height="423" alt="image" src="https://github.com/user-attachments/assets/80829117-3365-4dfe-b51e-7ebc0393fdc8" />

**SPIE Poster: 2026 Photonic Europe**

Following Book proposal is under review:
**SPIE Spotlights: State-Aware World Models for Nanophotonic Design:Dynamic Field Prediction, Structural Editing, and Digital-Twin Foundationsn**

