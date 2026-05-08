# MigraCast – Developer Workflow Guide

## Purpose of this Guide

This document defines:
- development order
- AI workflow strategy
- implementation phases
- repository organization
- chat usage strategy
- project priorities

The goal is to develop MigraCast in a structured and scalable way while using AI tools efficiently.

---

# Core Development Philosophy

## Important Principle

Do NOT try to build the entire system at once.

MigraCast should be developed iteratively:

1. planning
2. data understanding
3. baseline ML
4. prototype UI
5. integration
6. optimization
7. personalization

---

# AI Workflow Strategy

## Chats should have ONE clear purpose only.

Bad:
- "Build the entire app"

Good:
- "Help me preprocess the migraine dataset"
- "Help me build the Streamlit input form"
- "Help me improve model evaluation"

---

# Context Strategy

Every new AI chat should receive:

- PROJECT_CONTEXT.md
- CURRENT_STATE.md
- ARCHITECTURE.md
- DATASETS.md
- TASK.md

The AI should first summarize:
- project understanding
- current state
- risks
- proposed implementation strategy

before implementation starts.

---

# Recommended Development Order

---

# Phase 1 – Data Understanding

## Goal

Understand all datasets before coding complex systems.

---

## Tasks

### 1. Load datasets
Create:
- notebook for exploration
- dataset inspection
- column overview

### 2. Analyze datasets
Inspect:
- missing values
- feature distributions
- label balance
- correlations

### 3. Create initial visualizations
Examples:
- migraine occurrence frequency
- stress vs migraine
- sleep vs migraine

---

## Recommended AI Chat Goal

"Help me perform EDA on the migraine dataset."

---

# Phase 2 – Preprocessing

## Goal

Create clean ML-ready datasets.

---

## Tasks

### 1. Clean data
- missing values
- duplicates
- datatype fixes

### 2. Feature engineering
Examples:
- normalize features
- encode categories
- create combined weather features

### 3. Create train/test split

---

## Recommended AI Chat Goal

"Help me build a preprocessing pipeline using pandas and sklearn."

---

# Phase 3 – Baseline ML Model

## Goal

Build the first working migraine prediction model.

---

## Tasks

### 1. Logistic Regression
Use as baseline model.

### 2. Evaluate metrics
Track:
- accuracy
- recall
- F1-score

### 3. Analyze feature importance

---

## Important Principle

The first model does NOT need to be perfect.

The goal is:
- working pipeline
- understandable logic
- measurable output

---

## Recommended AI Chat Goal

"Help me train and evaluate a baseline logistic regression model."

---

# Phase 4 – Streamlit Prototype

## Goal

Build first interactive frontend.

---

## Tasks

### 1. Create input form
Potential inputs:
- sleep
- stress
- hydration
- screen time

### 2. Display prediction
Show:
- migraine probability
- risk level

### 3. Add visualizations
Examples:
- feature importance
- trends

---

## Important Principle

Focus on:
- simplicity
- usability
- functionality

NOT on:
- perfect design
- advanced animations

---

## Recommended AI Chat Goal

"Help me build a simple Streamlit frontend for the prediction pipeline."

---

# Phase 5 – Weather Integration

## Goal

Integrate external environmental features.

---

## Tasks

### 1. Open-Meteo API integration
Fetch:
- temperature
- humidity
- pressure
- precipitation

### 2. Connect weather to prediction pipeline

---

## Recommended AI Chat Goal

"Help me integrate Open-Meteo weather data into the prediction system."

---

# Phase 6 – User Tracking

## Goal

Store user history and enable personalization.

---

## Tasks

### 1. Store user entries
Initial idea:
- CSV
Possible future:
- SQLite

### 2. Create trend analysis

### 3. Analyze recurring patterns

---

## Recommended AI Chat Goal

"Help me implement local user tracking and history storage."

---

# Phase 7 – Personalization

## Goal

Adapt predictions to individual users.

---

## Planned Concepts

- adaptive feature weighting
- user-specific trigger analysis
- retraining on personal history

---

## Important Note

This is an advanced phase.
Do NOT start here.

---

# Repository Workflow

## Branch Strategy

Recommended branches:
- main
- development
- feature/*

Examples:
- feature/preprocessing
- feature/streamlit-ui
- feature/weather-api

---

## Commit Philosophy

Commit small logical changes.

Good:
- "Add preprocessing pipeline"
- "Implement logistic regression baseline"

Bad:
- "stuff"
- "update"

---

# Documentation Workflow

After every major step:

Update:
- CURRENT_STATE.md
- ROADMAP.md

Optional:
- TASK.md

---

# Recommended Chat Structure

## Example Workflow

### Chat 1
EDA + data understanding

### Chat 2
Preprocessing pipeline

### Chat 3
Baseline model

### Chat 4
Model evaluation

### Chat 5
Streamlit frontend

### Chat 6
Weather integration

### Chat 7
Persistence + tracking

---

# Important Technical Priorities

## Focus first on:

1. clean data
2. working ML pipeline
3. understandable predictions

NOT on:
- complex UI
- authentication
- cloud infrastructure
- mobile apps

---

# Most Important Principle

MigraCast is primarily:
- a predictive analytics project
- a decision support system
- a Business Informatics ML project

NOT:
- a medical product
- a diagnosis tool

---

# Final Development Philosophy

The goal is NOT to create the most complex system.

The goal is to create:
- a clean architecture
- a working ML workflow
- understandable predictions
- a scalable foundation for future extensions