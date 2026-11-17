# VENTUSAI — Wind Turbine Intelligence Center

**CAI 401 · Group 4 · Section 72U · Princess Nourah bint Abdulrahman University**

A two-stage machine-learning research prototype for anomaly detection and fault classification using wind turbine SCADA data.

## Project

- 10 turbines (WT01–WT10), 260,367 cleaned SCADA records, 48 sensor features
- Stage 1: Random Forest binary Normal/Fault detection (compared with Isolation Forest)
- Stage 2: SVM (RBF) three-class fault diagnosis (compared with XGBoost and Random Forest)
- Target fault classes: Lubrication, Electrical, Generator_Cooling

### Held-out test results

| Evaluation | Metric | Score |
|---|---|---:|
| Stage 1 | Fault F1 | 2.10% |
| Stage 2 independent on known faults | Macro F1 | 69.90% |
| Two-stage end-to-end | Macro F1 | 43.80% |
| Two-stage end-to-end | Accuracy | 87.77% |

The weak Stage 1 test fault detection limits end-to-end usefulness. The current system is **an academic prototype, not validated industrial monitoring or safety-critical software**.

## Live demonstration

**[Open VENTUSAI](https://alshehrilama74-M.github.io/VENTUSAI/)**

The web dashboard displays offline evaluation metrics and **rule-based simulated** sensor scenarios. These simulations do not run the trained Random Forest/SVM models live.

## Files

- `code/CAI401_Group4_Preprocessing_72U.ipynb` — SCADA cleaning, labeling and splitting.
- `code/CAI401_Group4_Final_ML_Code_72U.ipynb` — model training, comparison and testing.
- [DATA.md](DATA.md) — dataset inputs, provenance and reproducibility notes.
- [DEMO.md](DEMO.md) — dashboard walkthrough.

The source files required to re-run the notebooks are not automatically included in this repository. See DATA.md and ensure the preprocessing output partition matches the final evaluation partition.

## Team

Shahad Alanazi · Lama Alshehri · Rana Alashur · Lina Albdrani

Course: CAI 401 · Group 4 · Section 72U.
