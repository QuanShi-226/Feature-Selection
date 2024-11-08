# Feature Selection Comparison for Breast Cancer Classification

This repository contains a comprehensive report and Jupyter Notebook for comparing three feature selection methods—Recursive Feature Elimination (RFE), SelectFromModel, and a custom Genetic Algorithm—applied to the Breast Cancer dataset. This project demonstrates how different feature selection techniques impact model performance, feature interpretability, and dataset dimensionality.

## Project Overview

**Objective**: To evaluate and compare the effectiveness of different feature selection methods for classifying breast cancer tumors as malignant or benign. This includes:
- Reducing the dimensionality of the dataset while maintaining high model accuracy.
- Identifying the most representative and interpretable features.
- Analyzing the stability and redundancy of selected feature sets.

### Methods Compared

1. **Recursive Feature Elimination (RFE)** - A wrapper method that iteratively removes the least important features based on model weights.
2. **SelectFromModel** - An embedded method that filters features based on model coefficients, selecting the most important features in a single pass.
3. **Genetic Algorithm (GA)** - A custom GA that evolves feature subsets based on model performance and a feature count penalty.

### Dataset

The Breast Cancer dataset from Scikit-learn was used, containing 30 features that describe characteristics of cell nuclei in breast cancer biopsies. The target variable classifies tumors as malignant or benign.

## Repository Structure

- `report.pdf`: A detailed report comparing the three feature selection methods across several dimensions:
  - Number of features selected
  - Model performance (accuracy, precision, recall, F1-score)
  - Feature importance and representativeness
  - Stability and reproducibility
  - Handling of feature correlation and redundancy
- `Feature_Selection_Comparison.ipynb`: The Jupyter Notebook with code implementations for RFE, SelectFromModel, and Genetic Algorithm, including data processing, model training, and evaluation.

## Key Findings

- **SelectFromModel** emerged as the best method, achieving a good balance between feature reduction and model performance. It selected only 9 features, simplifying the model while maintaining high accuracy and interpretability.
- **RFE** achieved slightly higher accuracy but retained more features, resulting in a more complex model with potential redundancy.
- **Genetic Algorithm** offered a balanced approach, selecting 13 features with comparable performance to RFE and SelectFromModel, though with higher variability due to randomness in the selection process.

## Usage

To explore the code and analysis:
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Feature-Selection-Comparison-Breast-Cancer-Classification.git
