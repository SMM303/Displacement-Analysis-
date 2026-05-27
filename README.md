# Displacement-Analysis-
WB data analysis
# Displacement Analysis: Machine Learning and Humanitarian Risk

## Overview

This repository contains the complete Python analytical pipeline supporting
the chapter:

**Beyond Prediction: Machine Learning, Adaptation Finance, and the
Governance of Climate-Driven Internal Displacement**

Published in: *Advancing the Environmental SDGs Through Science, Law
and Data*. Taylor & Francis / Routledge, 2026.

Author: Saleh Mansour

---

## Repository Contents

| File | Description |
|---|---|
| WB_Data.ipynb | Main Jupyter notebook — full analysis pipeline |
| DISPLACEMENT_MASTER.csv | Master analytical dataset (147 countries, 25 variables) |
| requirements.txt | Python package versions used in the analysis |
| README.md | This file |

---

## Data Sources

The master dataset integrates two open-access sources:

**IDMC Global Internal Displacement Database (GIDD), 2025**
Disaggregated displacement events: 21,340 events across 149 countries.
Available at: https://www.internal-displacement.org/database/displacement-data

**INFORM Risk Index, 2026**
191-country coverage across 286 risk indicators aggregated into
10 composite dimensions.
Available at: https://drmkc.jrc.ec.europa.eu/inform-index

---

## Analytical Methods

The notebook implements six complementary methods in sequence:

1. Exploratory data analysis and distributional profiling
2. Spearman rank correlation analysis
3. Random Forest regression with SHAP value decomposition
4. K-means clustering with silhouette optimization
5. Logistic regression classification (AUC-ROC = 0.973)
6. Principal Component Analysis

---

## Key Findings

- INFORM Overall Risk correlates with total new displacements
  at rho = 0.603 (p < 0.001)
- Weather-related events account for 65.6 percent of all
  disaggregated displacement incidents
- Coping capacity is the strongest structural moderator of
  displacement outcomes across all six methods
- The logistic classifier achieves cross-validated AUC = 0.920
  (plus or minus 0.056)
- One principal component explains 50.3 percent of variance
  in the INFORM risk indicator set

---

## How to Run

**Requirements**

Python 3.9 or later. Install dependencies with:

```bash
pip install -r requirements.txt
```

**Running the notebook**

```bash
jupyter notebook WB_Data.ipynb
```

All cells run sequentially. Data files must be placed in the
same directory as the notebook or paths adjusted accordingly.

---

## Citation

If you use this code or data in your own research, please cite:

Mansour, S. (2026) 'Beyond Prediction: Machine Learning,
Adaptation Finance, and the Governance of Climate-Driven
Internal Displacement', in *Advancing the Environmental SDGs
Through Science, Law and Data*. London: Taylor & Francis /
Routledge.

**SMM303 (2026) “SMM303/Displacement-Analysis-: Version 1.0 — Chapter Submission Release”. Zenodo. doi:10.5281/zenodo.20414956.**
---

## License

This repository is shared under the MIT License.
See LICENSE file for details.

---

## Contact

For questions about the analytical pipeline, please open an
issue in this repository.
