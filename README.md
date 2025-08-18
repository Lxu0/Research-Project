# Research Project: SSCWT Analysis of HD 174966

## Overview
This repository contains the code and Jupyter notebook for my MSc research project on the non-stationary pulsation behaviour of the δ Scuti star **HD 174966** using the **Synchrosqueezed Continuous Wavelet Transform (SSCWT)**.  
It reproduces the main findings of Ramon-Ballesta et al. (2022) and provides quantitative validation (anti-correlation, dropouts, and approximate total-power constancy) for two low-frequency modes.

## Repository Structure
```
├── research-project.ipynb   # Main analysis notebook 
├── data/                    # Input data (see below)
├── figures/                 # Figures saved by the notebook
├── requirements.txt         # Python dependencies
└── README.md
```

## Data

The analysis relies on CoRoT photometric data of HD 174966 provided in MATLAB `.mat` format.  
A sample `.mat` file is included in the `data/` directory so that the notebook can be executed and tested.  

The full dataset is available from the [CoRoT Public Archive](http://idoc-corot.ias.u-psud.fr/).
For full replication, please download the original CoRoT light curve and place it in the `data/` directory using the same filename convention.


## Requirements
Python 3.10+  
Install dependencies:
```bash
pip install -r requirements.txt
```
Minimal packages:
- numpy
- pandas
- scipy
- matplotlib
- ssqueezepy
- jupyter (to run the notebook)

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the notebook:
   ```bash
   jupyter notebook research-project.ipynb
   ```
4. Run all cells to reproduce the analysis and regenerate figures (saved to `figures/`).

## Key Outputs
- SSCWT time–frequency maps (scalograms) of HD 174966  
- Band-energy time series for 5.51 and 6.30 d⁻¹  
- Dropout statistics, ridge connectivity, and anti-correlation metrics  
- Approximate constancy of combined power across the two modes
