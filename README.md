# ITAGAKI-SYSTEM FOR MICROBIOLOGY
### Physical-Diagnostic Framework for Compositional Data Analysis on Microbiology
**Compositional data** is defined as data in which variables are normalized within each sample and the sum of the variables is a constant.

## Overview
**ITAGAKI-SYSTEM** is a rigorous computational framework developed to overcome the fundamental limitations of compositional data analysis in biological sciences. Conventional statistical methods (PCA, Pearson Correlation, CLR-transform) often fail or produce spurious results when dealing with datasets characterized by **extreme scale gaps (10^1 to 10^11)** in sample total abundance (Effective Library Size).

This system bypasses mathematical illusions by anchoring all diagnostics to **Physical Reliability Mapping** and **Poisson Noise Floor** constraints. It ensures that biological interpretations are based on physical reality rather than sampling artifacts.

---

## Core Modules

### 1. [Ver.2] Physical Reliability Mapping
Evaluates the quantitative validity of each component per sample by dynamically calculating the **Poisson Noise Floor (1/Eff_Lib)**.
- **Key Feature:** Classification into *Reliable* (≥10x Floor), *Uncertain* (Presence only), and *Absent*.
- **Purpose:** To prevent "noise-driven" conclusions in low-depth samples.

### 2.  [V8.1-LOO] Physical Integrity & Stability Tracker
A **Leave-One-Out (LOO)** perturbation analysis designed to identify specific samples (rows) that destabilize the physical integrity of the entire system.
- **Key Feature:** **Normalized Score** generation. Scores > 2.0 trigger a "Physical Integrity Alert."
- **Purpose:** Automated detection of measurement errors, data entry mismatches, or extreme biological shifts.

### 3. [V18.1] Physical Coherence Engine (Integrated)
Tests the **Subcompositional Invariance** of the system by stripping the top 10% "Physical Drivers" (high-IR components) and measuring the structural stability of the remaining core.
- **Key Feature:** **Physical Rho** (IR-based Spearman rank correlation).
- **Purpose:** To identify key biological drivers (columns) and verify the robustness of the underlying physical architecture.

---

## Why Physics over Statistics?
In microbiology and nutrition science, the "Total" is often an artifact of the measurement process (e.g., sequencing depth). **ITAGAKI-SYSTEM** treats every sample as a unique physical entity with its own precision limit. By normalizing variance against the theoretical **Poisson limit**, the system enables fair comparison across samples with vastly different scales.

## Academic Citation
If you use this software or its logic in your research, please cite the following works:
- **Ohta, T. (2011)**. DOI: 10.1007/s11004-011-9332-y
- **Itagaki, T (2024)**. DOI: 10.3390/microorganisms12071484
- **Itagaki, T (2025)**. DOI: 10.3390/nu17233681
---

## License
Copyright (c) 2026 Tatsuki Itagaki.  
Licensed under the **MIT License**.

**Developed by:** Tatsuki Itagaki  
**Version:** 2026.4.27 (Production Ready)
