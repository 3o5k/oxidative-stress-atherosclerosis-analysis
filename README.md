# Oxidative Stress Biomarker Analysis in Atherosclerosis
### Python-based Statistical & Multivariate Analysis Pipeline

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Lab-orange?logo=jupyter)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
Complete statistical analysis pipeline for a master's thesis investigating 
the **protective and therapeutic effects of N-Acetylcysteine (NAC)** against 
vitamin D3/high-fat-diet-induced atherosclerosis in Sprague-Dawley rats.

> Manuscript under review — *Pharmacological Research* (IF 7.0)

## Biomarkers
| Marker | Full Name | Role |
|---|---|---|
| MDA | Malondialdehyde | Lipid peroxidation index |
| GSH | Reduced Glutathione | Non-enzymatic antioxidant |
| GpX | Glutathione Peroxidase | Peroxide scavenging |
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

## Notebooks
| Notebook | Contents |
|---|---|
| 01_data_cleaning.ipynb | Raw Excel → clean CSV |
| 02_statistical_analysis.ipynb | Shapiro-Wilk, Levene, ANOVA, Tukey HSD, CLD |
| 03_visualisation.ipynb | Bar charts, Boxplots, Heatmap, PCA, Regression |

## Key Findings
- Atherogenic induction raised MDA by **~77%** and depleted SOD by **~82%**
- High-Dose NAC normalised GSH, GRD, and MDA to normal control levels
- PCA: PC1 captures **>80% of total variance** across all five biomarkers
- SOD predicts serum MDA concentration (R² > 0.60, p < 0.001)

## Tech Stack
`Python 3.10` · `Jupyter Lab` · `pandas` · `NumPy` · `SciPy` · 
`statsmodels` · `scikit-learn` · `Matplotlib` · `Seaborn` · `NetworkX`

## Author
**Abdulmuhsen Almutairi**  
MSc Biochemistry — University of Jeddah, Saudi Arabia  
📧 m7sen.1223@gmail.com
