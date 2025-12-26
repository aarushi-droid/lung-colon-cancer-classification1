# lung-colon-cancer-classification
# Lung and Colon Cancer Classification using Deep Feature Fusion

This project focuses on multi-class classification of lung and colon cancer histopathological images using deep learning–based feature extraction, feature selection, and an MLP classifier.

---

## Overview
- Pre-trained CNNs (MobileNetV2 and ResNet50) are used as feature extractors
- Extracted features are fused and reduced using statistical feature selection
- A Multi-Layer Perceptron (MLP) classifier is trained on the selected features
- Model performance is evaluated using accuracy, precision, recall, F1-score, ROC, and PR curves

---

## Dataset
- Lung and Colon Cancer Histopathological Images
- Source: Kaggle
- Classes:
  - Colon Adenocarcinoma
  - Colon Benign Tissue
  - Lung Adenocarcinoma
  - Lung Benign Tissue
  - Lung Squamous Cell Carcinoma

---

## Methodology
1. Image preprocessing and resizing
2. Feature extraction using MobileNetV2 and ResNet50
3. Feature fusion (concatenation)
4. Feature selection using:
   - SelectKBest (ANOVA F-score)
   - Recursive Feature Elimination (RFE)
5. Feature ranking and top-N selection
6. Classification using MLP
7. Comprehensive evaluation and visualization

---

## Tech Stack
- Python
- TensorFlow / Keras
- Scikit-learn
- OpenCV
- NumPy, Pandas
- Matplotlib, Seaborn

---

## How to Run
```bash
pip install -r requirements.txt
python src/cancer_classification.py
