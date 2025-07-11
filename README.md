🌾 Impacts of Climate Change on Spatial Wheat Yield and Nutritional Values Using Hybrid Machine Learning
📄 Environmental Research Letters, Vol. 19, 104049 (2024)
📌 DOI: 10.1088/1748-9326/ad57f9

This repository provides the full code, data structure, and modeling workflow for predicting the impacts of climate change on wheat yield and grain nutritional traits (protein, iron, zinc) across Egypt using a hybrid machine learning framework. The models integrate observed phenotypic data with CMIP6-based climate scenarios under both SSP2-4.5 and SSP5-8.5.

🌐 Project Overview
The study responds to urgent global needs for:

Climate-resilient crop forecasting

Site-specific nutrition-smart agriculture

Scalable methods to assess micronutrient gaps under warming climates

We built a hybrid machine learning pipeline that combines:

📊 Ground-truth wheat data: Grain yield, protein, Fe, Zn

🌡 CMIP6 downscaled climate data (historical, mid-century, end-century)

🧠 Traditional ML models (RF, ANN, SVR, DT, KNN)

⚙️ Automated Machine Learning (AutoML) tools for optimized model stacking and tuning

🗂 Repository Structure
pgsql
Copy
Edit
├── Climate_Wheat_HybridML.ipynb           # Main notebook for model training and projections
├── data/
│   ├── crop_traits.csv                    # Wheat yield, protein, Fe, Zn (field data)
│   ├── climate_features_baseline.csv      # Historical climate inputs
│   ├── cmip6_ssp245_midcentury.csv        # SSP2-4.5 scenario input
│   ├── cmip6_ssp585_endcentury.csv        # SSP5-8.5 scenario input
├── outputs/
│   ├── predictions_maps/                  # Spatial outputs and visualizations
│   └── model_performance.csv              # R², RMSE, feature importance
├── figures/                               # Final figures from publication
└── README.md                              # This file
🔧 Modeling Approach
Feature Engineering

Climate variables (temp, precip, humidity, solar radiation)

Derived indices and regional encoding

Hybrid Modeling

Comparison of individual models and AutoML-stacked models

Repeated cross-validation with optimized hyperparameters

Scenario Projections

Yield and quality mapped under baseline, SSP2-4.5, SSP5-8.5

Temporal comparison (2020–2049 vs 2070–2099)

