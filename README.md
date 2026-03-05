# Tobacco Mortality Forecasting Using Machine Learning

## Project Overview

Smoking-related diseases remain a major contributor to global mortality and healthcare burden. Predicting future mortality trends can help public health organizations allocate resources and design effective interventions.

This project builds a **machine learning model to forecast next-year smoking-related mortality rates** using historical smoking prevalence and hospital admission data.

The project demonstrates a **complete end-to-end data science workflow**, including data preprocessing, feature engineering, exploratory data analysis, model training, and interpretation of results.
## Project Preview

<p align="left">
  <img src="reports/figures/Cigarette-photo.jpeg" width="450">
  <img src="reports/figures/pipe_tobacco.jpg" width="450">
</p>
---

## Problem Statement

Smoking contributes significantly to hospital admissions and mortality worldwide. Healthcare planners need tools to **anticipate future mortality burden** in order to allocate medical resources and design preventive strategies.

The objective of this project is to **predict next-year smoking-related mortality rates** using historical data such as:

- Smoking prevalence by age group  
- Smoking-related hospital admissions  
- Demographic segments  
- Historical mortality trends  

---

## Business Understanding

Public health agencies can use predictive models to:

- Forecast healthcare burden  
- Plan medical resource allocation  
- Monitor long-term smoking trends  
- Identify high-risk population segments  

This model provides **predictive insights to support decision-making**, rather than causal explanations.

---

## Dataset Description

The dataset is created by combining multiple public health data sources.

### Admissions Dataset
Contains yearly data on **smoking-related hospital admissions**.

### Fatalities Dataset
Contains yearly data on **smoking-attributable deaths**.

### Smokers Dataset
Provides **smoking prevalence across different age groups**, including:

- 16–24  
- 25–34  
- 35–49  
- 50–59  
- 60+  

These datasets were merged to create a **year-based dataset with demographic and health indicators** used for modeling.

---

## Project Workflow

The project follows a standard **machine learning pipeline**:

1. Data Collection  
2. Data Cleaning  
3. Dataset Merging  
4. Feature Engineering  
5. Exploratory Data Analysis (EDA)  
6. Train-Test Split  
7. Model Training  
8. Model Evaluation  
9. Feature Importance Analysis  

---

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand patterns in smoking prevalence and mortality trends.

### Key Observations

- Smoking rates have generally declined over time.  
- Mortality trends show patterns related to smoking prevalence.  
- Certain age groups demonstrate stronger associations with mortality outcomes.  

EDA helps identify relationships between features and supports better model development.

---

## Feature Engineering

To prevent **data leakage**, the target variable was shifted to represent **next-year mortality rate**.

### Key Engineered Features

- Mortality rate calculated as **fatalities / admissions**  
- **Lagged mortality features** to capture historical trends  
- Smoking prevalence across age groups  
- Demographic segment (sex)

These features help the model capture temporal patterns and improve predictive performance.

---

## Modeling

A machine learning pipeline was implemented using **Scikit-learn**.

### Models Evaluated

- Random Forest Classifier  
- Logistic Regression  

### Key Techniques Used

- Time-aware validation  
- Machine learning pipelines  
- Permutation feature importance for model interpretability  

---

## Results

The model successfully captures relationships between smoking prevalence and mortality trends.

### Key Findings

- Smoking prevalence in **older age groups** is strongly associated with mortality outcomes.  
- **Hospital admissions** serve as a strong predictor of future mortality trends.  
- **Lagged mortality features** improve predictive performance.

These insights demonstrate how historical public health data can support predictive modeling for health outcomes.

---

## Key Visualizations

The project includes several visualizations to support analysis and interpretation:

- Smoking prevalence trends over time  
- Mortality rate trends  
- Feature importance plot  
- Correlation heatmap of variables  

These visualizations help explain the relationship between smoking behavior and mortality patterns.

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  
- Seaborn
