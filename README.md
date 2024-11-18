# Car Price Prediction
### Author: Virendrasinh Chavda

This repository contains an end-to-end machine learning project to predict car prices using various regression models. The project includes data preprocessing, feature selection, dimensionality reduction, and performance evaluation of models. Additionally, the effects of log transformation and dimensionality reduction techniques on the models are analyzed.

---

## Table of Contents
1. [Overview](#overview)
2. [Installation](#installation)
3. [Features](#features)
4. [Usage](#usage)
5. [Methodology](#methodology)
6. [Results](#results)
7. [Future Work](#future-work)
8. [Contributing](#contributing)
9. [License](#license)

---

## Overview

<p align="justify">
The Car Price Prediction project utilizes multiple regression models to predict car prices based on various features such as engine specifications, dimensions, and car type. The project evaluates the impact of dimensionality reduction techniques and log transformations on model performance using metrics like R-Squared score. Additionally, visualizations such as correlation heatmaps, bar plots, and feature importance charts are used to interpret the results.
</p>

---

## Installation

To set up and use this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/VirendraChavda/Price-Prediction.git
   cd car-price-prediction
   ```
2. Launch the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
## Features

### Dimensionality Reduction Analysis
- Evaluated the impact of dimensionality reduction techniques:
  - Correlation-based dimensionality reduction.
  - Lasso-based dimensionality reduction.
- Analyzed performance using R-Squared scores for different models.

### Feature Selection
- Identified important features using Lasso regularization.

### Visualization
- Generated a heatmap to visualize feature correlations.

### Log Transformation Effect
- Evaluated the impact of log transformation on R-Squared scores for different models.

---

## Usage

### Data Preprocessing
- Use `Car Price Prediction.ipynb` to:
  - Clean and preprocess the datasets (`CAR DETAILS FROM CAR DEKHO.csv`, `car data.csv`, etc.).
  - Apply transformations such as log scaling and encoding.

### Feature Selection
- Perform feature selection using Lasso regularization.

### Model Training and Evaluation
- Train regression models (Linear Regression, SVM, KNN, Random Forest, etc.) using the preprocessed data.
- Compare R-Squared scores with and without dimensionality reduction.

### Visualization
- Visualize the results using heatmaps, bar plots, and feature importance charts.

---

## Methodology

### Steps

#### Data Preprocessing
- Handle missing values and encode categorical features.
- Apply log transformation to the target variable (`Price`) to normalize its distribution.

#### Dimensionality Reduction
- Reduce features using correlation analysis and Lasso-based feature selection.

#### Model Training
- Train models such as Linear Regression, SVM, KNN, Decision Trees, Random Forest, Gradient Boost, XGBoost, and AdaBoost.

#### Evaluation
- Evaluate models using R-Squared scores and compare performance with dimensionality reduction and log transformations.

#### Visualization
- Generate correlation heatmaps and feature importance charts.

---

## Results

### Dimensionality Reduction Impact
- Models performed consistently better with Lasso-based dimensionality reduction compared to correlation-based reduction.
- R-Squared scores improved significantly for most models after dimensionality reduction.

### Log Transformation Impact
- Applying log transformation to the `Price` column improved R-Squared scores for most models.

### Feature Importance
- Features like `Year`, `Model`, `Fuel Type`, `Transmission`, and engine specifications (`Max Power`, `Max Torque`) were identified as the most significant predictors of car prices.

---

## Future Work

### Advanced Models
- Explore advanced regression models like LightGBM or CatBoost for better performance.

### Feature Engineering
- Incorporate additional features like resale value, service history, or customer reviews.

### Deployment
- Deploy the model as a web app using Flask or Streamlit for real-time predictions.

---

## Contributing

Contributions are welcome! Feel free to fork the repository, make improvements, and submit a pull request. If you encounter any issues, open a GitHub issue for discussion.

---

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.
