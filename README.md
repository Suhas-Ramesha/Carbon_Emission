# 🌍 Climate Change Data Analysis & CO₂ Emission Prediction

This project aims to analyze country-specific climate change data and build machine learning models to **predict CO₂ emissions** using multiple country-level parameters. The data is sourced from the **World Bank Climate Change Data Catalog**, spanning **1990–2011**, and includes diverse indicators such as greenhouse gas emissions, population statistics, economic metrics, land usage, and more.

---

## 🧠 Project Overview

### 🔹 Data Source
- Dataset: [Climate Change Data by World Bank Group](https://datacatalog.worldbank.org/dataset/climate-change-data)
- License: [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)
- File: `climate_change_download_0.xls`

### 🔹 Problem Statement
To build data-driven models that **predict CO₂ emissions** using historical country-level data related to:
- Greenhouse gases (CO₂, CH₄, N₂O)
- Population (total, urban, growth)
- Economic indicators (GDP, GNI, FDI)
- Land use (agriculture, protected areas)
- Energy use, climate data (precipitation, disasters)
- Health infrastructure

---

## 🔄 Project Stages

### 📌 Stage 1: Data Cleaning and Preparation
> Location: `notebooks/Stage1_Data_Cleaning_and_Preparation.ipynb`

- **Global Data Overview**  
  Insight into raw dataset shape (13,512 rows × 28 columns), types, and feature scope.

- **Data Cleaning Steps**:
  - Removed rows/columns with only null or placeholder ("..") values
  - Converted object-type numeric values to float
  - Filtered out irrelevant features (`SCALE`, `Decimals`, etc.)
  - Renamed and restructured long feature names
  - Transformed wide data format into a melted format per country-year-variable

- **Final Output**: Cleaned DataFrame saved as `Cleaned_Data.csv`

---

### 📌 Stage 2: Data Exploration and Predictive Modeling
> Location: `notebooks/Stage2_Data_Exploration_and_Prediction.ipynb`

- **Exploratory Data Analysis (EDA)**:
  - Distribution and correlation analysis of emissions vs. other indicators
  - Feature selection and engineering

- **Machine Learning Models**:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting
  - Model evaluation using RMSE, R², etc.

- **Objective**: Predict **CO₂ emissions (EN.ATM.CO2E.KT)** using selected socio-economic and environmental features.

---

## 🧪 Installation & Usage

1. Clone this repository:
```bash
git clone https://github.com/your-username/climate-co2-prediction.git
cd climate-co2-prediction
```

Set up your environment:
```bash
Copy
Edit
pip install -r requirements.txt
```

Launch Jupyter Notebook:
```bash
Copy
Edit
jupyter notebook
```

Explore notebooks:

Stage1_Data_Cleaning_and_Preparation.ipynb

Stage2_Data_Exploration_and_Prediction.ipynb

## 📊 Sample Features Used
Population

Urban population

GDP ($)

Energy use per capita

Methane (CH4) emissions

Nitrous oxide (N2O) emissions

Agricultural land (%)

Nationally protected areas (%)

## 📈 Results
The best-performing model demonstrated a strong predictive capability for CO₂ emissions using a combination of economic, demographic, and environmental indicators. Visualizations and metrics are available in the Stage 2 notebook.

## 🚀 Future Work
Incorporate more recent data (post-2011)

Include satellite data or external APIs for real-time updates

Apply deep learning models (e.g., LSTM for temporal prediction)

Develop an interactive dashboard (e.g., using Streamlit)

## 📚 References
World Bank Group Climate Change Data: https://datacatalog.worldbank.org/dataset/climate-change-data

CO₂ Emissions Definitions: IPCC Guidelines

Pandas Documentation: https://pandas.pydata.org/

## 📬 Contact
Author: [Suhas Ramesha
Email: rsuhas319@gmail.com
LinkedIn: linkedin.com/in/suhas-ramesha/
