# **Crime Through the Years: Unveiling Trends and Patterns**

A comprehensive analysis of crime data from Prince George's County, Maryland (2017–2024) to identify trends, predict crime types, and create actionable insights for public safety and policymaking. This project combines machine learning models, statistical analyses, and visualizations to explore crime patterns.

---

## **Project Overview**

This project aims to analyze crime trends, forecast future incidents, and classify crime types using advanced statistical techniques and machine learning models. It incorporates geospatial and temporal data to provide insights into crime hotspots and patterns.

Key questions addressed:
- How have crime trends evolved over time?
- Can crime types be predicted based on incident features?
- Which regions have higher crime rates, and do they correspond to specific crimes?

---

## **Dataset**
Crime data for this project was sourced from the [Prince George's County Open Data Portal](https://data.princegeorgescountymd.gov/). The data spans February 2017 to September 2024 and includes information on:
- Crime types (e.g., theft, assault, vandalism)
- Incident locations (latitude, longitude, reporting areas)
- Dates and times of incidents
- Clearance codes and other incident metadata

**Key Details**:
- Total records: **184,583**
- Preprocessing steps:
  - Standardized and cleaned column names
  - Handled missing values and duplicates
  - Merged two datasets for a unified analysis

---

## **Features**
### **Statistical Analyses**
- **Chi-Square Test**: Analyzed relationships between incident types, years, and reporting areas.
- **ANOVA**: Tested the variance of incident frequencies over time.

### **Machine Learning Models**
- **SARIMA Model**:
  - Forecasted crime trends with seasonal and temporal components.
  - Achieved low error rates (MSE: 96,908.49; RMSE: 311.30).
- **KNN Classifier**:
  - Predicted incident types, achieving optimal performance with k=18.
- **Decision Tree & Random Forest**:
  - Classified crime types based on geospatial and temporal data.
  - Enhanced performance using SMOTE to handle imbalanced classes.
- **Neural Network**:
  - Explored multi-class classification with deep learning but required further optimization.

### **Clustering Analysis**
- **K-Means Clustering**:
  - Identified crime hotspots with cluster severity scores.
- **PCA**:
  - Reduced dimensionality for better visualization of clustering results.

### **Visualizations**
- Temporal trends of crime incidents (2017–2024).
- Monthly crime rates and seasonal patterns.
- Interactive maps showing incident distributions and localized crime clusters.

## **Results**
- **SARIMA Model**: 
  - Forecasted crime frequencies over time, identifying seasonal patterns and long-term trends.
  - Achieved low error rates with MSE: 96,908.49, RMSE: 311.30.
- **KNN Classifier**: 
  - Achieved optimal accuracy with k=18, performing well for frequent crime types.
  - Struggled with minority classes due to imbalanced data.
- **Random Forest**: 
  - Improved classification performance using SMOTE and feature engineering.
- **Visualization Insights**: 
  - Identified crime hotspots and seasonal patterns using interactive maps and temporal analyses.

## **Technologies Used**
- **Languages**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras, GeoPandas
- **Tools**: Jupyter Notebook, SMOTE, Plotly
- **Techniques**: SARIMA, KNN, Random Forest, PCA, K-Means, Data Visualization


## **Contributors**
- **Berkay Yenilmez**: Developed SARIMA models, KNN classifiers, and visualizations for temporal and geospatial analyses.
- **Dimitri Duron**: Assisted with dataset selection, Random Forest modeling, and documentation.
- **Neha Dutt**: Conducted EDA, model evaluations, and contributed to decision tree and neural network models.
- **Manuela Deigh**: Created visualizations, contributed to clustering and PCA, and helped prepare the final report.
- **Siva Buthada**: Focused on data preprocessing, data cleaning, and data curation for analysis readiness.

