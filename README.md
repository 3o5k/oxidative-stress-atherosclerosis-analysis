# Oxidative Stress Biomarker Analysis in Atherosclerosis
### Python-based Statistical & Multivariate Analysis Pipeline

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Lab-orange?logo=jupyter)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
Statistical analysis pipeline for my MSc thesis, *Relationship between N-acetylcysteine and atherosclerosis in rats*, which examines the protective and therapeutic effects of N-acetylcysteine (NAC) against vitamin D3/high-fat-diet-induced atherosclerosis in Sprague-Dawley rats.

> Manuscript in preparation.

## Biomarkers
| Marker | Full Name | Role |
|---|---|---|
| MDA | Malondialdehyde | Lipid peroxidation index |
| GSH | Reduced Glutathione | Non-enzymatic antioxidant |
| GPx | Glutathione Peroxidase | Peroxide scavenging |
| GRD | Glutathione Reductase | GSH recycling |
| SOD | Superoxide Dismutase | Primary ROS defence |

## Experimental Groups
| Group | Treatment |
|---|---|
| Normal Control | Standard diet + saline |
| Atherosclerotic Control | HFHC diet + Vitamin D3 |
| Low-Dose NAC | HFHC + 150 mg/kg/day NAC (prophylactic) |
| High-Dose NAC | HFHC + 300 mg/kg/day NAC (prophylactic) |
| NAC Treatment | HFHC + 300 mg/kg/day NAC (therapeutic) |

n = 5 animals per group.

## Notebooks
| Notebook | Contents |
|---|---|
| `01_create_dataset.ipynb` | Raw Excel → clean CSV |
| `02_statistical_analysis.ipynb` | Shapiro-Wilk, Levene, one-way ANOVA, Tukey HSD, compact letter display |
| `03_visualisation.ipynb` | Bar charts, boxplots, correlation heatmap, PCA, regression |

## Data
The raw experimental data are unpublished and are not included in this repository. `data/dummy_biomarker_data.xlsx` is an illustrative file with the same structure, so the pipeline can be run end to end. To reproduce the analysis on it, rename it to `raw_biochemistry_data.xlsx` before running `01_create_dataset.ipynb`.

## Key Findings
- Atherogenic induction raised MDA by **~77%** and depleted SOD by **~82%**
- High-dose NAC returned GSH, GRD and MDA to normal control levels
- PCA: PC1 captures **81.3% of total variance** across all five biomarkers
- SOD predicts serum MDA concentration (R² = 0.623, p < 0.001)

## Tech Stack
`Python 3.10` · `JupyterLab` · `pandas` · `NumPy` · `SciPy` · `statsmodels` · `scikit-learn` · `NetworkX` · `Matplotlib` · `Seaborn`

## Author
**Abdulmohsen Almutairi**
MSc Biochemistry & Bioinformatics, University of Jeddah, Saudi Arabia
abdulmohsen.khalef@gmail.com

## License
MIT. See [LICENSE](LICENSE).
