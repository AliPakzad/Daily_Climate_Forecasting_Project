# Daily_Climate_Forecasting_Project

## Introduction

This notebook analyzes and models the **Daily Climate Time Series Dataset** from Delhi, India — available on [Kaggle](https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data).  
The dataset provides daily observations of **mean temperature**, **humidity**, **wind speed**, and **mean pressure** from **January 2013 to April 2017**.

---

### 🎯 Project Objective
The main goal is to **forecast the daily mean temperature** using deep learning–based time series models implemented in the **Darts** library.

---

### 🧠 Models Used
Four different models are developed and compared:
- **DeepAR**
- **N-BEATS**
- **Temporal Fusion Transformer (TFT)**
- **DeepTCN**

---

### ⚙️ Methodology
For each model:
- Models are optimized for **forecast horizon = 10 days**
- Evaluation metrics such as **MAE** and **MAPE** are computed on the validation set.
- A **backtesting** procedure is also performed to assess temporal prediction stability.
- The effect of adding different **covariates** on forecasting performance is analyzed:
  - **Past covariates:** humidity, wind speed, mean pressure  
  - **Future covariates:** month and season (derived from the `date` column)

---

Finally, all four models are compared to study:
- The impact of adding past and future covariates  
- The relative forecasting performance of DeepAR, N-BEATS, TFT, and DeepTCN  

This notebook provides a complete workflow for multivariate time series forecasting and model comparison using real-world climate data.
