# This Project is for analyzing and modeling

# Folder structure

### 1. Dataset folder
- raw data
- data cleaned
- link resouche from kaggle

### 2. data_preparation.ipynb
-  notebook for cleaning feature extraction, and preparing data for analysis purposes in Tableau

### 3. Tesla Global Data Analyst.twb
- The tableau file => analysis, Dashboard, Insights
- link to tableau public: https://public.tableau.com/views/TeslaGlobalDataAnalyst/KPIDashboard?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

### 4. regression.ipynb
- No missing values, no 
- Several columns are not normally distirbuted
- Based on Classical assumption test
    : Linearity (resid) => Linear
    : Normality (resid) => Not Normal
    : Multicolinearity => Severe multicol on Several columns
    : Heterokesdasisity => No Hetero
    : Autocorelation => No Autokor
- Multiple Linear Regression is rejected due to multicollinearity and non-normal residuals.
- Selected model: XGBoost Regressor, because it is robust to multicollinearity and non-normal feature distributions.
-  Model Evaluate:
    MAE : 213.1566925048828
    RMSE: 284.7688755815846
    R²  : 0.9945597648620605

