# MigraCast – Architecture

## High-Level Overview

MigraCast is structured as a modular predictive analytics system.

The architecture combines:
- frontend UI
- ML prediction pipeline
- external weather API
- local user tracking

---

## Frontend

Framework:
- Streamlit

Responsibilities:
- user input
- risk visualization
- trigger display
- charts and dashboards

---

## Backend

Language:
- Python

Libraries:
- Pandas
- NumPy
- Scikit-Learn

Responsibilities:
- preprocessing
- feature engineering
- prediction
- evaluation

---

## Machine Learning Pipeline

### Input
- lifestyle features
- health features
- weather data

### Processing
- preprocessing
- normalization
- feature selection

### Output
- migraine probability
- risk level
- feature importance

---

## Data Sources

### Internal
- user tracking data
- local CSV/database storage

### External
- Open-Meteo API

---

## Planned Prediction Flow

User Input
↓
Weather API
↓
Feature Processing
↓
ML Model
↓
Probability Prediction
↓
Visualization in Streamlit

---

## Planned Storage

Initially:
- CSV files

Possible future upgrade:
- SQLite
- PostgreSQL

---

## Explainability

Planned methods:
- feature importance
- probability explanation
- trigger visualization

Goal:
Users should understand WHY a prediction was made.

---

## Future Extensions

- wearable integration
- Apple Health integration
- recommendation engine
- personalized retraining
- cloud deployment