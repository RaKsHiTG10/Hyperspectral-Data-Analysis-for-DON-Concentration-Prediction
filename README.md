# Hyperspectral-Data-Analysis-for-DON-Concentration-Prediction
 This project focuses on processing hyperspectral imaging data to predict DON (vomitoxin) concentration in corn samples using machine learning. The steps include data preprocessing, dimensionality reduction, model training, and evaluation using XGBoost.
Data Preprocessing

Dropped identifier column (hsi_id)
Filled missing values with column means
Clipped outliers using 1st and 99th percentiles
Applied Box-Cox transformation to fix target skewness
Feature Scaling & Visualization

Scaled features using StandardScaler
Created line plot and heatmap for spectral reflectance
Dimensionality Reduction

Applied PCA (20 components)
Visualized top 2 components with explained variance
Model Training

Scaled target variable using StandardScaler
Trained XGBoost with RandomizedSearchCV for tuning
Model Evaluation

MAE: 3.4394 | RMSE: 4.5996 | R²: 0.2416
Scatter plot for actual vs. predicted values
Model Interpretability

Used SHAP to explain feature importance
SHAP summary plot for top influential features
 Results & Insights
Model performance shows moderate correlation (R² = 0.24)
SHAP analysis highlights key spectral bands influencing predictions
Future work: Try increasing PCA components, fine-tuning model, and exploring CNN or LSTM models
