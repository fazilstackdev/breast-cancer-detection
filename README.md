# 🎗️ Breast Cancer Detection - Multi-Model Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-green.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 🔬 A comprehensive machine learning project for breast cancer classification using multiple algorithms including KNN, Random Forest, Decision Tree, and SVM. Achieves high accuracy in distinguishing benign vs malignant tumors.

---

## 📊 Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Algorithms Used](#algorithms-used)
- [Model Performance](#model-performance)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)
- [Developer](#developer)

---

## 📋 Project Overview

This project implements **multiple machine learning algorithms** to classify breast cancer tumors as **Benign** (non-cancerous) or **Malignant** (cancerous). The goal is to build an accurate and reliable diagnostic tool using the Wisconsin Breast Cancer Dataset.

### Why This Project?
- Breast cancer is one of the most common cancers worldwide
- Early detection significantly improves survival rates
- Machine learning can assist doctors in making faster and more accurate diagnoses

---

## 📁 Dataset

**Source:** Wisconsin Breast Cancer Dataset (WBCD)

| Property | Value |
|----------|-------|
| **Samples** | 569 |
| **Features** | 30 (real-valued) |
| **Classes** | 2 (Benign, Malignant) |
| **Benign samples** | 357 (62.7%) |
| **Malignant samples** | 212 (37.3%) |

### Features include:
- Radius (mean of distances from center to points on perimeter)
- Texture (standard deviation of gray-scale values)
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Concave points
- Symmetry
- Fractal dimension

*... and their standard errors and worst values*

---

## 🤖 Algorithms Used

| # | Algorithm | Type | Description |
|---|-----------|------|-------------|
| 1 | **K-Nearest Neighbors (KNN)** | Instance-based | Classifies based on k closest training samples |
| 2 | **Random Forest** | Ensemble | Builds multiple decision trees and averages predictions |
| 3 | **Decision Tree** | Tree-based | Creates a tree-like model of decisions |
| 4 | **Support Vector Machine (SVM)** | Margin-based | Finds optimal hyperplane for classification |

### Additional Techniques:
- ✅ Data Preprocessing (StandardScaler normalization)
- ✅ Train-Test Split (80/20 ratio)
- ✅ Cross-Validation (5-fold)
- ✅ Hyperparameter Tuning (GridSearchCV)
- ✅ Feature Importance Analysis

---

## 📈 Model Performance

### Accuracy Comparison

| Algorithm | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|-----------|----------|-----------|--------|----------|---------|
| **KNN** | 95.6% | 0.95 | 0.96 | 0.95 | 0.97 |
| **Random Forest** | 96.5% | 0.96 | 0.97 | 0.96 | 0.98 |
| **Decision Tree** | 93.0% | 0.93 | 0.94 | 0.93 | 0.94 |
| **SVM** | 97.1% | 0.97 | 0.97 | 0.97 | 0.98 |

### 🏆 Best Model: **SVM with 97.1% accuracy**

### Confusion Matrix (SVM)