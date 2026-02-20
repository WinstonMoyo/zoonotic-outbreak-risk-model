# Zoonotic Outbreak Risk Model

## Overview

A **machine learning system** designed to model and forecast the risk of **zoonotic disease outbreaks** by simulating transmission across key ecological interfaces.

The project models pathogen spillover across three stages — **wildlife**, **livestock**, and **humans** — using separate predictive models combined through an **ensemble learning approach**. While trained on synthetic data, the feature design is informed by real-world ecological, environmental, and behavioral factors.

This project demonstrates how machine learning can be applied to **public health risk assessment and decision support**.

---

## Objectives

- Model zoonotic spillover across three transmission interfaces:
  1. Wildlife infection risk
  2. Wildlife-to-livestock transmission
  3. Livestock-to-human spillover
- Design ecologically informed features reflecting environmental and behavioral drivers
- Use ensemble learning to improve predictive performance
- Demonstrate end-to-end ML workflow for public health applications

---

## Technologies Used

- **Python 3**
- **scikit-learn** – model training and evaluation
- **XGBoost** – gradient boosting models
- **pandas**, **numpy** – data processing
- **matplotlib**, **seaborn** – visualization and analysis

---

## Model Architecture

The system is composed of three primary models, each representing a stage in the zoonotic transmission chain:

### 1. Wildlife Infection Risk Model
Predicts the probability of wildlife infection based on environmental factors such as habitat loss, climate variability, and proximity to human activity.

### 2. Wildlife-to-Livestock Spillover Model
Estimates transmission risk from wildlife to livestock using features such as species interaction frequency, land use, and biosecurity practices.

### 3. Livestock-to-Human Transmission Model
Models final spillover risk based on farming practices, food consumption behavior, and human susceptibility factors.

---

## Ensemble Strategy

Predictions from all three models are combined using an **ensemble classifier** to produce a final outbreak risk score.  
This approach improves robustness and reduces error compared to individual models.

---

## Results

- Final ensemble model accuracy: **~90.5%**
- Ensemble learning outperformed individual stage-specific models
- Confusion matrices and performance metrics indicate balanced classification behavior

---

## Limitations

- Training data is synthetic, though feature design is ecologically informed
- The model is not intended for real-world deployment without validation on empirical datasets

---

## Future Improvements

- Integrate real-world data sources (e.g. climate, land-use, and deforestation datasets)
- Extend the model to time-series forecasting
- Build a lightweight dashboard or API for risk visualization
- Explore deep learning approaches such as LSTM for temporal modeling
