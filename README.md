# SkyPredictor: Intelligent Weather Trend Forecasting System

## Overview

SkyPredictor is a data science project focused on analyzing and forecasting short-term weather trends using global weather data. The project explores how machine learning models can capture temporal patterns and environmental relationships to predict daily temperature trends.

This project demonstrates an end-to-end pipeline including:
1. Data cleaning and preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature engineering for time-series modeling
4. Forecasting with multiple machine learning models
5. Advanced analyses including anomaly detection and geographical pattern exploration

## Dataset
- Source: Global Weather Repository (Kaggle)
- Link: https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository?resource=download

Contains:
1. Weather metrics (temperature, humidity, pressure, wind, precipitation)
2. Air quality indicators (PM2.5, CO, NO₂, etc.)
3. Temporal features (last_updated)
4. Geographical data (latitude, longitude, country)


## Project Workflow

1. **Data Preprocessing**
- Handled missing values using median imputation
- Cleaned inconsistent country names (multilingual normalization)
- Converted timestamps into structured time features
- Removed duplicates and treated outliers using IQR

2. **Exploratory Data Analysis (EDA)**
- Analyzed distributions of temperature and precipitation
- Identified correlations between weather and air quality variables
- Explored geographical variations across countries

3. **Feature Engineering**
- Created lag features (previous observations)
- Generated rolling statistics for temporal patterns
- Incorporated environmental variables

4. **Modeling & Forecasting**

Implemented and compared multiple models:
- Baseline (Persistence Model)
- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor
- Ensemble Model

5. **Advanced Analysis**
- Anomaly Detection using Isolation Forest
- Geographical Pattern Analysis across countries and continents
- Environmental Impact Analysis (weather vs air quality)
- Feature Importance Analysis

## Evaluation Metrics:

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R^2 Score
- MAPE


## Key Insights
- Weather trends show strong temporal dependency, making lag features highly effective
- Tree-based models outperform linear models, indicating non-linear relationships
- Geographical location significantly influences weather patterns
- Ensemble models improve prediction stability
- Air quality variables show moderate correlation with weather conditions

## Limitations
- Dataset is not a continuous long-term time series
- Global aggregation reduces regional specificity
- Some inconsistencies in country naming required preprocessing
- Limited external climate features

## Future Work
- Region-specific forecasting models
- Integration of external climate datasets
- Deep learning approaches (e.g., LSTM, Transformers)
- Real-time forecasting pipeline

## Tech Stack
- Python
- Pandas 
- NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Country Converter

## Repository Structure

├── data/

├── notebooks/

│   └── weather_analysis.ipynb

├── outputs/

│   ├── plots/

│   └── results/

├── README.md

└── requirements.txt
>

## How to Run
Clone the repository:

```bash
git clone https://github.com/your-username/SkyPredictor.git
cd SkyPredictor
```

Install dependencies:
```bash
pip install -r requirements.txt
```

Run the notebook:
```bash
jupyter notebook
```

## Author
Chamani Shiranthika, PhD candidate, Simon Fraser University, Canada
