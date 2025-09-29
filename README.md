# 🌍 Air Quality Prediction in Bandar Lampung

This project analyzes and forecasts **Air Quality Index (AQI)** in Bandar Lampung using historical air pollution data (2022–2024).  
The goal is to **understand air quality trends**, categorize pollution levels, and build a **forecast model** to predict future air quality conditions.

## 👨‍💻 Authors

- **Annisa Zhafirah** – Universitas Lampung  
- **Muhammad Rafi Rizanda** – Universitas Lampung  

---

## 📌 Project Objectives
1. Perform **data cleaning & preprocessing** on the Bandar Lampung air quality dataset.  
2. Categorize air quality levels based on AQI standards.  
3. Visualize pollutant concentrations and AQI distribution.  
4. Forecast future AQI values to anticipate changes in air quality.  

---

## 🗂️ Dataset Overview
- **Source:** Air Quality Dataset, Bandar Lampung (Jan 2022 – Feb 2024)  
- **Size:** 17,076 rows × 11 columns (before cleaning) → 108 rows × 10 columns (after cleaning, resampled weekly).  

### Key Columns
- `datetime` → Date & time of measurement (2022-01-16 to 2024-02-04)  
- `PM10`, `PM25` → Particulate matter pollutants  
- `SO2`, `CO`, `O3`, `NO2` → Gas pollutants  
- `AQI` → Air Quality Index  
- `kualitas_udara` → Categorized air quality (Good, Moderate, Poor)  

---

## ⚙️ Data Preprocessing
Steps performed:
- Converted `datetime` column into proper **datetime format**.  
- Removed invalid rows (`NaT` values).  
- Filtered **numeric columns only** for resampling.  
- Resampled dataset into **weekly averages**.  
- Converted cleaned dataset into **integer format**.  

---

## 📊 Exploratory Data Analysis (EDA)
1. **AQI Statistics** – Summary statistics of Air Quality Index.  
2. **Pollutant Distribution** – Visualization of PM10, PM2.5, SO2, CO, O3, NO2 concentrations.  
3. **Air Quality Categorization**  
   - **Good:** AQI ≤ 50  
   - **Moderate:** 50 < AQI ≤ 100  
   - **Poor:** AQI > 100  
4. **Visualization** – Bar plots & distributions of AQI and categorized air quality.  

---

## 🔮 Forecasting Analysis
- Forecasting performed using **Prophet model**.  
- Results show **fluctuations in AQI** over the next year.  
- Predictions indicate periodic rises and falls in AQI driven by pollutant variations.  

📌 **Insight:**  
These forecasts can serve as a **foundation for public policy & urban planning** to mitigate negative health and environmental impacts from poor air quality.  

---

## ✅ Conclusion
- The model predicts that air quality in Bandar Lampung will continue to **fluctuate periodically**.  
- Forecast results suggest **episodes of increasing AQI** due to pollutant concentration.  
- Findings can be used by local government and communities for **planning activities, public health measures, and pollution mitigation strategies**.  

---

## 📦 Tech Stack
- **Python**  
- **Pandas & NumPy** – Data preprocessing  
- **Matplotlib & Seaborn** – Visualization  
- **Prophet** – Time series forecasting  
- **Jupyter/Colab** – Development environment  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/air-quality-prediction.git
   cd air-quality-prediction
