# Airline Customer Satisfaction Prediction

> A comprehensive machine learning solution for predicting airline customer satisfaction using classification models and data analytics.

## Overview

This project presents a complete machine learning model for predicting airline customer satisfaction. It analyzes 130,000+ passenger records and leverages customer demographics, travel characteristics, and service ratings to build highly accurate predictive models.

**🏆 Best Model:** Random Forest Classifier — **96.4% Accuracy**

## Dataset

The dataset comprises 130,000+ airline customer records with the following attributes:

| Feature | Description |
|---------|-------------|
| Gender | Customer gender (Male/Female) |
| Customer Type | Type of customer (Loyal/Disloyal) |
| Age | Customer age |
| Type of Travel | Travel purpose (Personal/Business) |
| Class | Ticket class (Economy/Business/First Class) |
| Flight Distance | Distance of the flight in miles |
| Service Ratings | Seat comfort, WiFi, Entertainment, Online support, etc. (14 features) |
| Delays | Departure and Arrival delays in minutes |
| **satisfaction** | Customer satisfaction (target variable) |

## Methodology

The project follows a structured machine learning pipeline:

1. **Data Loading & Exploration** — Load and analyze dataset characteristics
2. **Data Preprocessing** — Handle missing values and clean data
3. **Exploratory Data Analysis** — Visualize patterns across customer segments and services
4. **Categorical Encoding** — Label encode categorical features
5. **Outlier Treatment** — Apply IQR detection to identify and remove outliers
6. **Feature Selection** — Chi-Square test to select top 10 impactful features
7. **Model Development** — Train multiple classification algorithms
8. **Model Evaluation** — Compare performance using test set evaluation

## Model Performance Results

| Model | Accuracy | Key Insight |
|-------|----------|------------|
| Random Forest Classifier | ⭐ **96.36%** | Ensemble method with best generalization |
| AdaBoost Classifier | 95.60% | DecisionTree base, n_estimators=40, learning_rate=0.5 |
| Support Vector Classifier | 94.82% | Strong performance on classification task |
| Logistic Regression | 85.85% | Linear baseline model |

**Key Finding:** Random Forest Classifier achieved the highest accuracy at 96.4%, significantly outperforming all other models through ensemble learning.

## Technology Stack

- **Language:** Python 3
- **Data Processing:** pandas, numpy
- **Visualization:** matplotlib, seaborn, plotly
- **Machine Learning:** scikit-learn

## Getting Started

### Installation

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

### Execution

```bash
jupyter notebook Model.ipynb
```

## Project Structure

```
airline-customer-satisfaction/
├── Model.ipynb              # Complete analysis and modeling notebook
├── Invistico_Airline.csv    # Dataset (130,000+ customer records)
└── README.md                # Documentation
```
