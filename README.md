# Coronary Heart Disease Risk Prediction 

## Project Overview

The objective is to build predictive models that use demographic, behavioural, and biomedical data to help identify individuals at risk of developing CHD.

## Models Implemented

### Support Vector Machine (SVM)
- **Accuracy**: 60%
- **Precision (CHD-positive)**: 0.21
- **Recall (CHD-positive)**: 0.59
- **F1-Score**: 0.31
- **AUC**: 0.68

> SVM performed best in identifying high-risk individuals, with a good recall, vital in healthcare screening.

### Multilayer Perceptron (MLP)
- **Accuracy**: 85%
- **Precision / Recall / F1**: 0.00 (failed to predict any CHD-positive cases)
- **AUC**: 0.68

> Despite high accuracy, the MLP model was ineffective due to class imbalance, predicting only the majority class.

## Files in This Repo

- `Ian's Findings.pdf` – Report summarizing my models, evaluation metrics, and key insights.
- `SVM_Model.ipynb` – Jupyter notebook implementing the SVM model.
- `MLP_Model.ipynb` – Jupyter notebook implementing the deep learning model.
- `README.md` – This file.

## Dataset

- Dataset used: **Framingham Heart Study**
- Data is not included due to licensing. You can access it from:
  - [Framingham Study Official Site](https://framinghamheartstudy.org/)
  - [Alternative (Kaggle)](https://www.kaggle.com/datasets/)

## Tools & Libraries

- Python (Google Colab)
- Scikit-learn
- TensorFlow / Keras
- Pandas, NumPy
- Matplotlib, Seaborn

## Key Takeaways

- In healthcare ML tasks, **recall > accuracy** — it's more important to catch at-risk patients than to minimize false positives.
- Class imbalance must be handled carefully; deep learning models can struggle without proper balancing techniques.
- Simpler models like SVM can outperform deep neural networks on structured, tabular data.

## Getting Started

To run the notebooks:
1. Open with [Google Colab](https://colab.research.google.com/)
2. Upload or link to the Framingham dataset
3. Run all cells in the order provided
