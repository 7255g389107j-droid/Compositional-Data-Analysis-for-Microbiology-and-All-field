# Compositional-Data-Analysis-for-Microbiology
R framework for microbiome CoDA using Aitchison geometry and "Itagaki-System" logic. It treats zero as the absolute baseline, using the Poisson Noise Floor to classify taxa. Features: Reliability Mapping (Taxa validation), LOO-Stability Tracker (Sample QC), Subcompositional Coherence (Robustness), and Chaos Engine V8.0 (System diagnostics).
# Compositional Data Analysis for Microbiology

This R-based framework ensures the mathematical integrity of microbiome datasets by integrating Aitchison geometry with "Itagaki-System" logic. It avoids arbitrary zero-substitution, instead identifying the **Poisson Noise Floor** (1/Effective Library Size) to distinguish reliable signals from stochastic noise, where zero is treated as the absolute baseline.

## Core Features

*   **Reliability Mapping**: Calculates sample-specific noise floors to classify taxa as Reliable, Uncertain, or Absent.
*   **LOO-Stability Tracker**: Detects samples that disproportionately perturb the system’s geometric and physical equilibrium.
*   **Subcompositional Coherence**: Tests if structural signals survive the removal of volatile components, ensuring result robustness.
*   **Chaos Engine (V8.0)**: Diagnoses system stability via Physical (invariance), Geometric (entropy), and Statistical (Ohta’s asymmetry) metrics.

This pipeline provides a rigorous diagnostic environment to validate compositional coherence and filter out false positives.

## Academic Citation
If you use this software or its logic in your research, please cite:
*   Ohta, T. (2011). DOI: 10.1007/s11004-011-9332-y
*   Itagaki, T. (2024). DOI: 10.3390/microorganisms12071484
*   Itagaki, T. (2025). DOI: 10.3390/nu17233681
*   Itagaki, T. (2026). DOI: 10.13140/RG.2.2.21953.93284
*   Itagaki, T. (2026). DOI: 10.13140/RG.2.2.35015.25762

## License
MIT License - Copyright (c) 2026 Tatsuki Itagaki
