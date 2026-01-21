License: Creative Commons Attribution–NonCommercial 4.0 International (CC BY-NC 4.0).  
Commercial use is not permitted without explicit authorization.

---

## Repository Structure (Artifact Contents)

This artifact intentionally contains **only the files listed below**.

There is **no `figures/` or `tables/` directory** in the submitted artifact.  
All figures and tables are generated **at runtime inside the Jupyter notebook**.

### Contents

- README.md  
- LICENSE  
- CITATION.cff  
- KAS_Evidence.ipynb  
- kas-sampling-theorem-appendix

No additional scripts, datasets, or binaries are included or required.

---

## Important Note for Reviewers

- This artifact is **not a software library**.
- The **Jupyter notebook itself is the primary research artifact**.
- No pre-generated figures or tables are included by design.
- Running the notebook **top-to-bottom reproduces all figures, tables, and appendix validations** reported in the manuscript.

---

# Kolmogorov–Arnold–Siddarth Sampling Theorem (KAS)
## Reproducibility Artifact

This repository contains the official reproducibility artifact for the paper:

**Kolmogorov–Arnold–Siddarth Sampling Theorem**

The artifact consists of a **single, self-contained Jupyter notebook** that implements all simulations, empirical validations, figures, and tables supporting the theoretical claims of the paper.

The notebook directly corresponds to:
- Section 4 — Research Methodology  
- Section 5 — Results and Empirical Validation (Observables O1–O6)  
- Section 6 — Discussion and Future Directions  
- Appendix A — Empirical and stochastic validation (A.1–A.14)

All numerical values reported in the paper are computed from executed experiments and are not hard-coded.

---

## 📂 Notebook Contents

### `KAS_Evidence.ipynb`

This notebook reproduces **all empirical evidence** in the manuscript, including:

- RF signal generation at **10 MHz** and **1.75 GHz**
- Stochastic noise models:
  - Gaussian
  - Brownian (Wiener)
  - Gaussian mixture
- Finite-window functional evaluation:
  - Power
  - Lag-1 and lag-2 correlations
- Spline-based Kolmogorov–Arnold Network (KAN) estimators
- Observables **O1–O6**, including:
  - Sampling / cylinder approximation error
  - Noise averaging behavior
  - Noise robustness
  - Cross-frequency generalization
  - Comparison with Shannon-style (FFT-based) baselines
  - Modular error decomposition
- Automatically generated:
  - Fixed-number figures (as referenced in the paper)
  - Tables A.X / A.Xb (Monte Carlo replicated)

---

## ▶️ How to Run

### 1. Open the notebook
Open `KAS_Evidence.ipynb` in Jupyter Notebook or JupyterLab.

### 2. Execute all cells
Run the notebook **from top to bottom** without modification.

No additional configuration, downloads, or external data are required.

---

## Reproducibility Statement

- All experiments are fully deterministic up to controlled random seeds.
- The notebook executes on standard consumer-grade hardware (CPU-only).
- No internet access is required.
- All figures and tables are regenerated at runtime.

This artifact is designed to satisfy common reproducibility and artifact-evaluation criteria (Goodman et al., 2016; ACM/IEEE guidelines).

---

## How to Review (Editor & Reviewer Note)

**To reproduce all results reported in the paper, run `KAS_Evidence.ipynb` from top to bottom. All figures, tables, and appendix validations will be generated automatically.**

---

## Citation

If you use or reference this artifact, please cite:

**Siddarth Laxminarayanan**  
*Kolmogorov–Arnold–Siddarth Sampling Theorem*, 2026.  
Reproducibility Artifact.

Citation metadata is provided in `CITATION.cff`.

---

## Scope and Limitations

This artifact validates the KAS theorem for **bounded quadratic and bilinear RF functionals** under finite sampling and stochastic noise.  
It is not intended as a general-purpose DSP or neural-network library.

---

## Contact

Email : L.SIDDARTH@OUTLOOK.COM

For questions related to reproducibility or review, please use the GitHub issue tracker.

---

## Repository Structure (Single Source of Truth)

```text
KAS/
├── KAS_Evidence.ipynb    # Complete empirical evidence:
│                         # • Section 4 — Research Methodology
│                         # • Section 5 — Results (Observables O1–O6)
│                         # • Section 6 — Discussion
│                         # • Figures (fixed numbering)
│                         # • Tables A.X / A.Xb
│                         # • Appendix A empirical validation
│
├── CITATION.cff           # Machine-readable citation metadata
│                         # (GitHub / Zenodo compatible)
│
├── README.md              # Reproducibility and reviewer guidance

No external scripts, datasets, or preprocessing steps are required.

