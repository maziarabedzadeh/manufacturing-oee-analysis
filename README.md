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
# Siemens S7-1500 Conveyor Control System

This project demonstrates an industrial automation control system designed for a conveyor-based production line using **Siemens S7-1500 PLC logic**. The project simulates a real-world manufacturing scenario, focusing on safety, efficiency, and fault handling.



## Project Overview
The primary objective of this project is to showcase professional-grade PLC programming techniques. Even in a simulated environment using TIA Portal/PLCSIM, the logic follows industrial standards for conveyor automation, including manual/automatic operations and fail-safe interlocks.

## Key Features & Skills
- **PLC Logic:** Implementing Motor Seal-in logic and timer-based fault detection.
- **Safety Interlocks:** Emergency Stop (E-Stop) logic to ensure system integrity.
- **Auto/Manual Modes:** HMI-based operational mode selection.
- **Fault Handling:** Automated detection of "Conveyor Jam" via sensor timeouts.
- **KPI Tracking:** Production counting and alarm management.

## Sequence of Operation
1. **Mode Selection:** Operator selects Auto/Manual mode via HMI.
2. **Safety Check:** System confirms Emergency Stop is inactive.
3. **Start Sequence:** Start command energizes the Conveyor Motor.
4. **Processing:** Sensors detect products, incrementing the Production Counter.
5. **Fault Monitoring:** If Sensor 2 does not detect product movement within 5 seconds, a "Jam Alarm" is triggered, stopping the motor.

## I/O Mapping
| Address | Tag Name | Description |
|---|---|---|
| I0.0 | Start_PB | System Start Push Button |
| I0.1 | Stop_PB | System Stop Push Button |
| I0.2 | E_Stop | Emergency Stop |
| I0.3 | Sensor_Infeed | Product Detection Sensor |
| I0.4 | Sensor_Outfeed | Product Exit Sensor |
| Q0.0 | Conveyor_Motor | Conveyor Motor Output |
| Q0.1 | Alarm_Light | Fault Alarm Indicator |

## Technical Implementation
- **Hardware Simulation:** Siemens S7-1500 (via PLCSIM)
- **Software:** Siemens TIA Portal
- **Programming Language:** Ladder Logic (LAD)

## Contact
**Maziar Abedzadeh**
*Analytical Chemist & Aspiring Automation Engineer*