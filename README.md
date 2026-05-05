# ITAGAKI-SYSTEM FOR MICROBIOLOGY
### Physical-Diagnostic Framework for Compositional Data Analysis on Microbioology and All field 
**Compositional data** is defined as data in which variables are normalized within each sample and the sum of the variables is a constant.

I have established a definitive suite of algorithms to identify Invariant Components. In a world where each dimension of Euclidean space fluctuates independently, the only salvation is to discover the "Unchanging Dimension" (Invariant Component).By utilizing this invariant component as a fixed reference (Anchor), the Absolute Quantity Ratio can be reconstructed through ALR (Additive Log-Ratio) transformation applied exclusively to UTR (Universally Reliable Taxa)—defined as components with non-zero values and a signal strength at least 10x the noise floor in all samples.Without an invariant component, the system is reduced to mere Chaos or Noise, where no scientific understanding can be attained. One must accept the boundary of the unknown when the Invariance is absent from the Compositional Data.

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
1. **Pearson, K. (1897).**  [DOI: 10.1098/rspl.1896.0076](https://doi.org)
2. **Ohta, T.    (2011).**  [DOI: 10.1007/s11004-011-9332-y](https://doi.org)
3. **Itagaki, T. (2026).**  [DOI: 10.13140/RG.2.2.35655.05287](https://doi.org)
---

## License
Copyright (c) 2026 Tatsuki Itagaki.  
Licensed under the **MIT License**.

**Developed by:** Tatsuki Itagaki  
**Version:** 2026.4.27 (Production Ready)
