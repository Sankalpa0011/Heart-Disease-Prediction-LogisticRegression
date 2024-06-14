# Heart Disease Prediction using Logistic Regression

This project aims to predict heart disease using a logistic regression model. The dataset used for this project contains various health metrics and a target variable indicating the presence or absence of heart disease.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Introduction

Heart disease is a leading cause of death worldwide. Early prediction and diagnosis can save lives by allowing for timely intervention. This project uses logistic regression to build a predictive model for heart disease based on a set of health-related features.

## Dataset

The dataset used in this project is `heartdiseasedata.csv`, which contains the following features:
- `age`: Age of the patient
- `sex`: Sex of the patient (1 = male, 0 = female)
- `cp`: Chest pain type (4 values)
- `trestbps`: Resting blood pressure
- `chol`: Serum cholesterol in mg/dl
- `fbs`: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false)
- `restecg`: Resting electrocardiographic results (values 0, 1, 2)
- `thalach`: Maximum heart rate achieved
- `exang`: Exercise induced angina (1 = yes; 0 = no)
- `oldpeak`: ST depression induced by exercise relative to rest
- `slope`: Slope of the peak exercise ST segment
- `ca`: Number of major vessels (0-3) colored by fluoroscopy
- `thal`: Thalassemia (3 = normal; 6 = fixed defect; 7 = reversible defect)
- `target`: Diagnosis of heart disease (1 = presence; 0 = absence)

## Installation

To run this project, you'll need to have Python installed along with several libraries. You can install the required libraries using the following command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/heart-disease-prediction.git
    cd heart-disease-prediction
    ```

2. Ensure the dataset `heartdiseasedata.csv` is in the `./Datasets/` directory.

3. Run the Python script:
    ```bash
    python heart_disease_prediction.py
    ```

## Results

The model's performance is evaluated using the following metrics:
- **Accuracy**: The proportion of correctly classified instances.
- **Confusion Matrix**: A table that is used to describe the performance of a classification model.
- **Classification Report**: A detailed report showing precision, recall, F1-score for each class.
- **Cross-Validation**: The model's performance is validated using 5-fold cross-validation to ensure robustness.
- **ROC Curve**: A plot showing the true positive rate versus the false positive rate.

### Example Output

```
Accuracy on training data: 0.85
Accuracy on testing data: 0.87
Cross-validation scores: [0.83 0.85 0.86 0.82 0.84]
Mean cross-validation score: 0.84

Confusion Matrix:
[[20  5]
 [ 3 33]]

Classification Report:
              precision    recall  f1-score   support

           0       0.87      0.80      0.83        25
           1       0.87      0.92      0.89        36

    accuracy                           0.87        61
   macro avg       0.87      0.86      0.86        61
weighted avg       0.87      0.87      0.87        61
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---
