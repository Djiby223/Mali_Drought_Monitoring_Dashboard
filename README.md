# Mali_Drought_Monitoring_Dashboard
Automated Agricultural Drought Intelligence &amp; Early Warning System  An end-to-end data analytics and forecasting pipeline that synchronizes heterogeneous meteorological rainfall indicators (SPI) with satellite vegetative health indices (NDVI) to pinpoint and predict environmental risk.
Automated Agricultural Drought Intelligence & Early Warning System

An end-to-end data analytics and forecasting pipeline that synchronizes heterogeneous meteorological rainfall indicators (SPI) with satellite vegetative health indices (NDVI) to pinpoint and predict environmental risk.

## 📊 Key Features & Engineering
- **Data Synchronization**: Unified messy daily/pentad precipitation records and satellite NDVI metrics onto a common monthly timeline.
- **Multi-Window Drought Indices**: Automated rolling-window calculations for the Standardized Precipitation Index across short-term and long-term horizons (SPI-1, SPI-3, SPI-6).
- **Cross-Correlation Core**: Mathematically discovered an explicit **60-day lag time window** showing a peak correlation of **r = +0.860** between short-term moisture shifts and canopy response.
- **Predictive Engine**: Integrated an autoregressive multivariate forecasting model (R² = 0.845) capable of predicting upcoming agricultural failure bounds 3 months in advance.

---

## 🔍 Core Data Findings

### 1. The 60-Day Drought Fuse
Statistical analysis over the synchronized baseline records confirms that immediate moisture changes have near-zero contemporary correlation (+0.098) with current greenness. However, tracking a rolling 3-month window exposes a highly synchronized pattern. Water stress anomalies and moisture deficits impact regional vegetation canopy health precisely two months later. 

### 2. Multi-Month Predictive Scenarios (Early Warning Horizon)
Using our validated multivariate framework, the system evaluates three forward trajectories from the end of the historical baseline:
- **Dry Decay Path (SPI-3 ≈ -1.5)**: Triggers a rapid vegetation drop to **0.174** by month 2, breaching the critical **Agricultural Crash Boundary (NDVI = 0.200)**.
- **Climatic Normal Path (SPI-3 ≈ 0.0)**: Projects a standard seasonal winter decay to **0.232** before a normal spring green-up.
- **Accelerated Recovery Bound (SPI-3 ≈ +1.5)**: Predicts immediate stabilization at **0.281**, completely bypassing seasonal stress.

---

## 🛠️ Tech Stack & Dependencies
- **Core Languages**: Python 3.11+
- **Data Engineering**: Pandas, NumPy
- **Statistical Analytics**: SciPy (SPI distribution fitting)
- **Visualization**: Matplotlib, Seaborn
- **Dashboard Interface**: Streamlit

---

## 📁 Repository Structure
```text
├── data/
│   ├── raw/            # Original climate and NDVI source files
│   └── processed/      # Calculated monthly anomalies and SPI outputs
├── notebooks/
│   └── drought_analysis.ipynb  # Interactive data discovery step
├── app.py              # Main Streamlit web application source code
├── requirements.txt    # Project package dependencies
└── README.md           # Project summary and documentation (This file)
```

---

