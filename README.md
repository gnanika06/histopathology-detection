# Breast Cancer Histopathology Detection

## Overview
A deep learning model to classify malignant vs benign breast tissue from microscopic histopathology images. Built to assist in early cancer screening by automating pathologist-level image analysis.

## Tech Stack
- Python, PyTorch, CNN

## Problem Addressed
Medical datasets are heavily imbalanced — far fewer malignant samples than benign. Most models fail here by optimizing for accuracy alone. This project tackles that using weighted loss functions, prioritizing recall because in healthcare, a false negative costs a life.

## Methodology
- Preprocessed histopathology image dataset
- Built CNN architecture for binary classification
- Addressed class imbalance via weighted loss
- Evaluated using F1-score and AUC-ROC (not just accuracy)

## Results
- **F1-Score: 90.99%**
- Evaluation metrics: F1, AUC-ROC, Confusion Matrix
- **Dataset:** Breast Histopathology Images (Invasive Ductal Carcinoma)

## Key Learning
Standard accuracy is misleading in medical ML. A model that predicts everyone as benign gets high accuracy but fails completely. F1-score and AUC-ROC reveal the truth.

## Dataset
Kaggle: Breast Histopathology Images (IDC)
https://www.kaggle.com/datasets/paultimothymooney/breast-histopathology-images

## How to Run
```bash
pip install torch torchvision
python train.py
```
