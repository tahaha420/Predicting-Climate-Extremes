# 🌡️ Predicting-Climate-Extremes
Heatwave and drought detection in Pakistan using XGBoost and Open-Meteo data

This project aims to improve the accuracy of climate forecasts in Pakistan by combining traditional weather prediction data with machine learning models. Specifically, it targets **heatwave detection** and **drought classification** using daily meteorological parameters sourced from **Open-Meteo**.  

We trained and evaluated ML models on a **per-province basis**, building separate pipelines for both tasks using engineered features and publicly available weather data.

---

## 📂 Repository Structure
├── model_training/
│   ├── heatwave/         # Jupyter notebooks for heatwave model training (per province)
│   └── drought/          # Jupyter notebooks for drought model training (per province)
│
├── datasets/
│   ├── raw/              # Original Open-Meteo data
│   └── processed/        # Feature-engineered datasets
│
├── trained_models/
│   ├── heatwave/         # Trained XGBoost models (saved as .pkl)
│   └── drought/          # Trained XGBoost models (saved as .joblib)
│
├── requirements.txt
└── README.md



---

## 🌐 Data Source

- **Provider:** [Open-Meteo](https://open-meteo.com/)
- **Granularity:** Daily
- **Features include:**
  - Maximum and minimum temperature
  - Precipitation
  - Relative humidity
  - Wind speed
  - Soil moisture
  - SPEI (for drought classification)
  - Others derived via feature engineering

---

## 🤖 Models and Results

### 🔥 Heatwave Detection
- **Model:** XGBoost
- **Target:** Binary (Heatwave / No Heatwave)
- **Accuracy:** ~80% on average across all provinces
- **Output:** Saved as `.pkl` files

### 🌵 Drought Classification
- **Model:** XGBoost
- **Target:** Multi-class (SPEI-based drought categories)
- **Accuracy:** ~94% on average across all provinces
- **Output:** Saved as `.joblib` files

---


