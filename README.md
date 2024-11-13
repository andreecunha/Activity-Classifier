# Activity-Classifier: Human Activity Recognition Pipeline

**Activity-Classifier** is a comprehensive pipeline for human activity recognition using data collected from wearable sensors. The project involves data preparation, feature engineering, and classification to identify distinct human activities. The solution is built with Python and integrates advanced data processing, feature extraction, and machine learning techniques.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Key Features](#key-features)
3. [System Workflow](#system-workflow)
4. [Installation Guide](#installation-guide)


---

## Project Overview

The project tackles the challenge of recognizing human activities using data collected from five sensors, including accelerometers, gyroscopes, and magnetometers. The dataset contains 16 distinct activities performed by 15 participants. The main objectives are:
- Data preparation: handling outliers, normalization, and transformation.
- Feature extraction: deriving meaningful temporal and spectral features.
- Classification: using machine learning models to predict activities.

---

## Key Features

1. **Data Preparation:**
   - Removal and handling of outliers using Z-score and clustering techniques.
   - Injection of synthetic outliers for robustness testing.

2. **Feature Engineering:**
   - Extraction of temporal and spectral features, including PCA and ReliefF.
   - Calculation of Fourier Transform and wavelet-based time-frequency matrices.

3. **Machine Learning Classification:**
   - Implementation of Support Vector Machine (SVM) models.
   - Evaluation using Train-Test (TT) and Leave-One-Subject-Out (LOSO) validation methods.

4. **Evaluation Metrics:**
   - Precision, Recall, F1-Score, and Confusion Matrix.

---

## System Workflow

1. **Data Loading:**
   - Load the FORTH-TRACE dataset from provided CSV files.

2. **Data Preprocessing:**
   - Normalize and clean the data.
   - Handle outliers and split data into training and testing sets.

3. **Feature Extraction:**
   - Calculate statistical features, spectral features (DFT), and time-frequency features (wavelets).

4. **Feature Selection:**
   - Apply PCA and Fisher Scores to select the most relevant features.

5. **Model Training and Testing:**
   - Train SVM classifiers with varying feature subsets.
   - Evaluate performance using TT and LOSO methods.

---

## Installation Guide

1. Clone the repository:
   ```bash
   git clone https://github.com/andreecunha/Activity-Classifier.git
