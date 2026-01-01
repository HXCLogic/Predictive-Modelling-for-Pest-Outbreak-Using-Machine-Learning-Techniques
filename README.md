# Predictive Modelling for Pest Outbreak Using Machine Learning Techniques

This repository contains the code, data, and supporting material for a research project on predicting rice pest outbreaks using machine learning.

The project uses a multi-year rice pest monitoring dataset (ICAR-CRIDA) and several supervised learning models to forecast weekly pest outbreak risk based on weather, temporal, and categorical variables.

## Repository contents

- `Rice.ipynb`  
  End-to-end Jupyter Notebook that implements the full workflow:
  - Data loading and exploratory analysis  
  - Feature engineering and target (Outbreak) definition  
  - One-hot encoding and train–test splitting  
  - Logistic Regression baseline model  
  - Random Forest and XGBoost ensemble models  
  - LSTM sequence model for a single pest–location series  
  - Model evaluation, cross-validation, feature importance, and plots  

- `data/`  
  Folder containing the curated rice pest dataset used in the notebook (e.g. `RICE.csv`).  

- `docs/` (optional, if present)  
  May include the dissertation PDF, pseudo-code (Appendix A), and any additional documentation or figures.

## Purpose

The main goals of this repository are to:

- Provide a transparent, reproducible implementation of the modelling pipeline described in the research report.  
- Demonstrate how standard machine learning and deep learning techniques can be applied to agricultural pest outbreak prediction.  
- Serve as a reference or starting point for researchers and practitioners interested in building data-driven pest forecasting or decision-support tools.

## Getting started

1. Clone this repository:
   ```bash
   git clone https://github.com/HXCLogic/Predictive-Modelling-for-Pest-Outbreak-Using-Machine-Learning-Techniques.git
   cd Predictive-Modelling-for-Pest-Outbreak-Using-Machine-Learning-Techniques
2. Create and activate a Python environment (for example, using venv or conda).
3. Install the required packages: "pip install -r requirements.txt"
4. Launch Jupyter and open Rice.ipynb

Then run the notebook cell by cell to reproduce the data preprocessing, model training, and evaluation results.

## Main models implemented
- Logistic Regression (baseline)
- Random Forest classifier
- XGBoost classifier
- LSTM sequence model for time-series outbreak prediction (single pest and location)

## Intended use
This code is intended for research, teaching, and experimentation. It is not a production-ready decision-support system. Any operational deployment should include additional data validation, calibration, and engagement with domain experts.
