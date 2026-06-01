# Integrated Population Viability Analysis (PVA): conservation portfolio evaluation

[![Website](https://img.shields.io/badge/Website-Live-brightgreen.svg)](https://annaortega-noaa.github.io/integrated_PVA_pipeline/)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)

> **[🌐 View the Full Interactive Pipeline & Documentation Here](https://annaortega-noaa.github.io/integrated_PVA_pipeline/)**

---

## Overview

This repository contains an integrated Population Viability Analysis (PVA) pipeline designed to evaluate conservation portfolios. The tool assesses both the impact of human-wildlife interactions ("takes") and the efficacy of proactive conservation strategies on the long-term survival of generic long-lived protected populations (e.g., marine turtles).

This 100% self-contained, synthetic data-free pipeline connects three distinct modeling phases:
1. **Data Imputation:** Filling gaps in historical nesting beach surveys using Bayesian state-space models via JAGS.
2. **Demographic Translation:** Implementing symmetric lifecycle algebra to convert "Takes" into "Adult Nester Equivalents" (ANE).
3. **Projection:** Simulating future population trends over a 100-year evaluation horizon across 8 unique management tracks (including nest protection, headstarting, anti-poaching, gear mitigation, safe handling, and a combined portfolio).

## Repository Structure

This project is built as a highly reproducible Quarto website. 
* **`_quarto.yml`**: The configuration file that dictates the website's structure and theme.
* **`*.qmd` files**: The interactive Quarto markdown files containing the R code, mathematical utilities, and narrative explanations for each phase of the pipeline.
* **`docs/`**: The rendered HTML files and assets deployed to GitHub Pages.

## How to Run Locally

To build and run this pipeline on your local machine:
1. Clone this repository.
2. Ensure you have R, RStudio, and JAGS installed.
3. Open the project directory in your terminal.
4. Run `quarto render` to execute the pipeline and build the website locally.

## Authors & Contributors

* **Anna Ortega** - Cooperative Institute for Marine & Atmospheric Research, University of Hawaiʻi at Mānoa, Honolulu, Hawaiʻi
* **Zachary Siders** - Fisheries and Aquatic Sciences Program, University of Florida, Gainesville, Florida
* **Summer Martin** - Protected Species Division, Pacific Islands Fisheries Science Center, National Marine Fisheries Service, National Oceanic and Atmospheric Administration, Honolulu, Hawaiʻi

## License & Disclaimer

As a work by US federal employees as part of their official duties, this project is in the public domain within the United States of America. We waive copyright and related rights in the work worldwide through the CC0 1.0 Universal public domain dedication.

*This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. All NOAA GitHub project code is provided on an 'as is' basis and the user assumes responsibility for its use. Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.*
