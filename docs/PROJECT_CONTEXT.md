# MigraCast – Project Context

## Project Overview

MigraCast is a Machine-Learning-based Streamlit application for predicting migraine risk probabilities based on lifestyle, health, and weather data.

The project is developed within the university module:
**Data Analytics & Big Data (Business Informatics, 4th semester).**

The goal is not just to track migraines retrospectively, but to proactively estimate migraine risks and identify individual triggers.

---

## Core Idea

The application combines:

- lifestyle data
- health-related data
- weather data
- machine learning

to calculate a daily migraine probability.

Example output:

> "Today's migraine risk: 72%
> Main factors: low sleep, high stress, air pressure drop."

---

## Main ML Question

How can lifestyle, health, and environmental data be combined to predict the probability of migraine attacks?

---

## Target Audience

- migraine patients
- health-tracking users
- users interested in preventive health analytics

---

## Main Features

- daily tracking
- migraine probability prediction
- trigger analysis
- weather integration
- feature importance visualization
- long-term pattern analysis

---

## Current Scope (MVP)

### Inputs
- sleep duration
- stress level
- hydration
- mood
- screen time
- weather data

### Outputs
- migraine probability
- risk level
- feature importance
- trigger explanations

---

## Main Datasets

### 1. Migraine Dataset from Wearable Devices

Main label:
`migraine_occurrence`

Relevant features:
- sleep_hours
- mood_level
- stress_level
- hydration_level
- screen_time
- migraine_severity

---

### 2. Sleep Health and Lifestyle Dataset

Additional features:
- Sleep Duration
- Quality of Sleep
- Physical Activity Level
- Heart Rate
- Daily Steps

---

### 3. Open-Meteo API

Weather features:
- temperature
- humidity
- air pressure
- precipitation

---

## Tech Stack

- Python
- Pandas
- Scikit-Learn
- Streamlit
- Open-Meteo API

---

## Planned ML Models

- Logistic Regression
- Random Forest
- optional: XGBoost

---

## Business Informatics Perspective

The project focuses on:
- predictive analytics
- decision support systems
- data integration
- explainable machine learning
- user-centered information systems

---

## Important Constraints

- not a medical diagnosis
- educational project
- predictions are probabilistic
- personalization requires long-term user data

---

## Current Status

- Q-phase completed
- datasets selected
- GitHub repository created
- Streamlit MVP generated