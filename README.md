# GridSense

---

## Problem Statement

Electric grids require accurate, short-term forecasts of renewable generation to maintain reliability and optimize dispatch. Forecast errors in solar and wind output lead to inefficient reserve allocation and increased balancing costs. This project builds a probabilistic forecasting system for renewable generation using weather model outputs and observational data, with an emphasis on uncertainty quantification.

## Why This Matters

Grid operators and energy traders rely on accurate forecasts to manage supply-demand balance in real time. Forecast errors can translate directly into financial losses through imbalance penalties and suboptimal dispatch decisions. Improving forecast reliability reduces operating costs and supports higher penetration of renewables.

## Approach

- **Data (planned):**
  - Numerical weather prediction (NWP) data (e.g., via Herbie)
  - Satellite-derived irradiance / wind fields
  - Historical generation or sensor data (solar/wind)
- **Feature engineering (planned):**
  - Time-aligned weather features
  - Site-specific transformations using PVLIB or windpowerlib
- **Modeling (planned):**
  - Deep learning models for time series forecasting (e.g., LSTM, temporal CNN)
  - Probabilistic methods (quantile regression, ensembles)
- **Evaluation (planned):**
  - Metrics: RMSE, CRPS, calibration curves
  - Reliability diagrams for probabilistic forecasts
- **Optimization layer (planned):**
  - Simple dispatch or bidding strategy based on forecast distributions
- **Outputs (planned):**
  - Point forecasts and prediction intervals
  - Interactive dashboard (Plotly/Dash or Streamlit)

## Current Status

Phase 1 — scoping data sources and system architecture

## Reproducibility

```
# Create environmentconda create -n gridsense python=3.10conda activate gridsense# Core dependenciespip install numpy pandas xarray torch plotly dash pvlib# (Planned) Ingest NWP and generation data# (Planned) Train forecasting models# (Planned) Launch dashboard locally
```
