# AGN Damped Random Walk (DRW) Modelling – ZTF Light-Curve Analysis

## Overview

This repository contains a reusable Python-based pipeline for analysing the optical variability of Active Galactic Nuclei (AGN) using long-term observations from the Zwicky Transient Facility (ZTF).

The project investigates five nearby Seyfert galaxies to understand their brightness variations and estimate their characteristic variability timescales using Damped Random Walk (DRW) modelling.

The analysis combines archival astronomical observations, data processing, statistical modelling and injection-recovery simulations to evaluate the reliability of the estimated timescales.

## Research Targets

The study investigates five Seyfert galaxies:

- NGC 4151
- NGC 5548
- Mrk 817
- NGC 4051
- NGC 7469

## Methodology

The pipeline follows these main steps:

1. **Data Retrieval:** Retrieves ZTF optical light-curve observations through the NASA/IPAC Infrared Science Archive (IRSA).
2. **Target Screening:** Examines source information and viewing-related factors that may affect the observed variability.
3. **Data Quality Assessment:** Identifies unreliable measurements and applies quality filters.
4. **Data Cleaning:** Removes poor-quality observations and combines repeated measurements from the same night.
5. **Light-Curve Visualisation:** Examines the temporal brightness variations of each target.
6. **DRW Modelling:** Applies Damped Random Walk modelling using Gaussian Processes and `celerite2`.
7. **Reliability Assessment:** Uses injection-recovery simulations to investigate the effects of sampling, measurement noise and finite observational baselines.

## Key Findings

The analysis produced characteristic damping timescales ranging approximately from **9.4 to 143 days** across the five studied galaxies.

These results provide insight into the optical variability of AGN and the behaviour of matter surrounding supermassive black holes.

## Technologies Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- SciPy
- Matplotlib
- Requests
- Astroquery
- celerite2
- Gaussian Process modelling
- ZTF Light-Curve API
- NASA/IPAC IRSA

## Repository Contents

| File | Description |
|---|---|
| `AGN_DRW_Pipeline New.ipynb` | Interactive Python notebook containing the reusable analysis pipeline. |
| `README.md` | Project overview, methodology and instructions. |

## How to Run

1. Clone or download this repository.
2. Install Python and Jupyter Notebook.
3. Install the required Python packages:

```bash
pip install numpy pandas scipy matplotlib requests celerite2 astroquery
```

4. Open the notebook:

```bash
jupyter notebook
```

5. Run `AGN_DRW_Pipeline New.ipynb` and follow the interactive prompts to configure the target and retrieve the observations.

## Data Sources

- [NASA/IPAC Infrared Science Archive (IRSA)](https://irsa.ipac.caltech.edu/)
- [Zwicky Transient Facility (ZTF)](https://www.ztf.caltech.edu/)
- [NASA/IPAC Extragalactic Database (NED)](https://ned.ipac.caltech.edu/)
- [SIMBAD Astronomical Database](https://simbad.cds.unistra.fr/simbad/)

## Research Purpose

This project demonstrates how publicly available astronomical survey data and computational modelling can be used to investigate the variability of active galaxies. The reusable pipeline is intended to support further analysis of AGN light curves and their characteristic variability timescales.

---

**Project:** AGN Damped Random Walk Modelling – ZTF Light-Curve Analysis  
**Research focus:** Active Galactic Nuclei, optical variability and stochastic modelling  
**Language:** Python
