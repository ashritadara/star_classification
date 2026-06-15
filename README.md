# star_classification

Machine learning project focused on classifying stars into different stellar categories using physical and observational properties such as temperature, luminosity, radius, magnitude, color, and spectral class.

Built and developed in Jupyter Notebook using Python-based data science and machine learning libraries for preprocessing, visualization, dimensionality reduction, model training, and evaluation.

---

## Overview

This project applies supervised machine learning techniques to classify stars into six different stellar categories. Multiple machine learning models were trained and evaluated to compare predictive performance across different algorithms.

Models implemented:
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree
- Random Forest
- Neural Network (MLP)

The primary goal was to determine which machine learning approach performs best on structured astrophysical data.

Random Forest achieved the strongest overall performance due to its ability to model complex non-linear relationships between stellar features.

---

## Dataset

Dataset Source:
https://www.kaggle.com/datasets/deepu1109/star-dataset

### Dataset Information
- Samples: 240
- Features: 7–9 (after feature engineering)
- Classes: 6

### Star Classes
| Label | Star Type |
|------|------------|
| 0 | Brown Dwarf |
| 1 | Red Dwarf |
| 2 | White Dwarf |
| 3 | Main Sequence |
| 4 | Supergiant |
| 5 | Hypergiant |

---

## Features Used

The models were trained using several physical and observational stellar properties:

- Temperature
- Luminosity
- Radius
- Absolute Magnitude
- Star Color
- Spectral Class

---

## Technologies & Libraries

### Environment
- Jupyter Notebook
- Python

### Data Processing
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn

### Machine Learning
- Scikit-learn

### Models & Techniques Used
- Logistic Regression
- Support Vector Machine (SVM)
- Decision Tree Classifier
- Random Forest Classifier
- Multi-Layer Perceptron (MLP)

### Dimensionality Reduction
- PCA (Principal Component Analysis)
- t-SNE

### Model Evaluation
- Confusion Matrix
- ROC Curve
- AUC Score
- Classification Report
- Cross Validation
- GridSearchCV

---

## Exploratory Data Analysis (EDA)

Performed:
- Feature distribution analysis
- Correlation heatmap
- HR diagram visualization
- Class imbalance analysis

Key observations:
- Luminosity and radius showed strong skewness
- Strong correlation between luminosity and radius
- Distinct stellar clusters appeared in the HR diagram

---

## Data Preprocessing

### Preprocessing Steps
- Label encoding categorical variables
- Feature scaling using standardization
- Stratified train-test split
- Log transformations for skewed features

### Feature Engineering
```python
log_luminosity = log(Luminosity + 1)
log_radius = log(Radius + 1)
