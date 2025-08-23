# Extremophile_ARG <img src="logo.png" alt="Project Logo" width="80" align="right" />

[![Code License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Content License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](LICENSE-CC-BY.md)
[![Made with R](https://img.shields.io/badge/Made%20with-R-276DC3.svg)](https://www.r-project.org/)

---

## Overview
This repository contains the reproducible analysis for **antimicrobial resistance genes (ARGs) in extremophiles**.  
The repo is organized to be lightweight and easy for reviewers to reproduce.

---

## Repository structure
```
Extremophile_ARG/
├── data/
│   ├── raw/           # Place original AMRFinder/other raw files here (not tracked)
│   └── processed/     # Generated intermediates (not tracked)
├── scripts/           # R Markdown / R scripts (tracked)
│   └── Extremophiles_ARG_Analysis.Rmd
├── results/
│   ├── tables/        # Final tables (generated)
│   └── figures/       # Final plots (generated)
├── README.md
├── LICENSE            # MIT (code)
└── LICENSE-CC-BY.md   # CC BY 4.0 (text/figures)
```
> Note: `data/` and `results/` are **not** pushed to GitHub (see `.gitignore`).

---

## How to reproduce
1. Clone the repository:
   ```bash
   git clone https://github.com/absartalat/Extremophile_ARG.git
   cd Extremophile_ARG
   ```
2. Open `Extremophiles_ARG.Rproj` in RStudio (or set the working directory to the project root).
3. Place input files under `data/raw/` (see `data/README.md` for details).
4. Run `scripts/analysis.Rmd`.  
   Outputs will be written to `results/tables/` and `results/figures/`.

---

## Requirements
- R (≥ 4.0)
- Suggested packages: `tidyverse`, `readr`, `dplyr`, `stringr`, `ggplot2`, `here`  
  (The Rmd prints `sessionInfo()` to record exact versions.)

---

## Data availability
Raw data are **not** included in this repository. See `data/README.md` for where to download and how to place them locally before running the analysis.

---

## Citation
If you use this repository, please cite:  
**Talat, A.** (2025). *ARGs in Extremophiles: Reproducible Analysis Pipeline*. GitHub: absartalat/Extremophile_ARG.

---

## License
- **Code** is licensed under **MIT** (see [`LICENSE`](LICENSE)).
- **Text, figures, and non-code assets** are licensed under **Creative Commons Attribution 4.0 International** (see [`LICENSE-CC-BY.md`](LICENSE-CC-BY.md)).

CC BY 4.0 badge and details: <https://creativecommons.org/licenses/by/4.0/>

---

## Contact
Maintainer: **Absar Talat** · GitHub: [@absartalat](https://github.com/absartalat)
