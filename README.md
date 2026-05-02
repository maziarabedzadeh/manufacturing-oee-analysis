# manufacturing-oee-analysis
Python-based analysis of production line efficiency (OEE) and downtime reduction
# Manufacturing OEE Analysis

## Objective
This project demonstrates the application of Python to analyze production line efficiency (OEE) and identify bottlenecks in a manufacturing environment.

## Key Skills Used
- **Data Analysis:** Processed shift-based production data using Pandas.
- **KPI Calculation:** Calculated Availability, Performance, and Quality metrics.
- **Automation Insight:** Visualized downtime patterns to support decision-making.

## Tools
- Python (Pandas, Matplotlib)
- Excel (Data Preparation)

## How it works
The script processes raw production logs (CSV) to calculate the OEE score and generates performance visualizations. This approach helps in transitioning from manual reporting to automated, data-driven process improvement.
# Manufacturing OEE Analysis

## Overview
This project simulates and analyzes a production line's Overall Equipment Effectiveness (OEE). It transforms raw shift-based production logs into actionable engineering insights to identify bottlenecks.

## Prerequisites
To run this analysis, you need Python installed on your system.

### Libraries Used (Install these)
You need to install the following dependencies:
```bash
pip install pandas matplotlib numpy
# Glioblastoma Microstructure Analysis (Ivy GAP)

## Overview
This project performs an end-to-end transcriptomic analysis of Glioblastoma (GBM) tumors using the **Ivy Glioblastoma Atlas Project (Ivy GAP)** dataset. The study maps how gene expression shifts across five distinct anatomical tumor regions, from the dense hypoxic core to the invasive leading edge.

## Methodology
The analysis pipeline involves:
- **Quality Control (PCA):** Principal Component Analysis to verify that biological structure (not patient demographics) drives sample variability.
- **Differential Expression (DESeq2):** Identification of "Star Genes" (e.g., *RAB3B*, *GABRA6*) that define distinct molecular signatures between tumor regions.
- **Network Analysis (WGCNA):** Co-expression network construction to reveal functional "engines" driving tumor biology:
    - **Blue Module (Angiogenic Engine):** Drivers of blood vessel growth (*KDR/VEGFR2*).
    - **Turquoise Module (Infiltration Engine):** Programs for brain-mimicry and spread (*CHKA*, *SYP*).

## Key Findings
- **Molecular Heterogeneity:** Two distinct molecular profiles separate the core from the invasive edge, suggesting region-specific therapeutic targets.
- **Tumor Mimicry:** GBM hijacks the brain's own neurotransmitter machinery (e.g., GABA/Glutamate pathways) to facilitate infiltration.

## Technical Stack
- **Languages:** R (v4.5.3+)
- **Packages:** `DESeq2`, `WGCNA`, `biomaRt`, `ggplot2`, `dplyr`

## Results
![PCA Plot](PCA_Plot.png)
![Volcano Plot](Volcano_Plot.png)

## Acknowledgements
Special thanks to Professor Nihal Salem for the guidance, mentorship, and scientific direction throughout this analysis.
