# ML_alrIEEEna_abhai

# IEEE ML Challenge – Device Fault Detection

## Overvieww

This project was developed as part of the **IEEE SB GEHU ML Challenge Qualifiers**.
The objective of this challenge is to build a **machine learning model that detects faulty devices** using sensor-based features.

Each device record contains **47 numerical features (F01–F47)** collected from an embedded monitoring system.
The model predicts whether the device is operating normally or experiencing a fault condition.

---

## Problem Statement

Given 47 sensor-based numerical features, the task is to classify the device state into:

* **0 → Normal device operation**
* **1 → Faulty device condition**

This is a **binary classification problem** evaluated using the **F1 Score**.

---

## Dataset Description

### TRAIN.csv

Used for training the machine learning model.

Contains:

* **F01 – F47** → sensor feature values
* **CLASS** → target label

### TEST.csv

Used for generating predictions.

Contains:

* **ID**
* **F01 – F47**

The task is to predict the **CLASS** column for the test dataset.

---

## Exploratory Data Analysis (EDA)

The following analysis was performed:

* Dataset overview and statistical summary
* Feature distribution analysis
* Class distribution visualization
* Correlation heatmap
* Feature importance evaluation

Visualizations were created using:

* **Matplotlib**
* **Seaborn**

---

## Machine Learning Approach

Steps followed in the modeling pipeline:

1. Data Loading
2. Exploratory Data Analysis
3. Feature Analysis
4. Model Training
5. Model Evaluation
6. Prediction on Test Dataset
7. Submission File Generation

---

## Model Used

The following algorithm was used for classification:

**XGBoost Classifier**

Reasons for choosing XGBoost:

* High performance on tabular datasets
* Handles numerical features efficiently
* Robust to feature interactions

---

## Evaluation Metric

The model performance is evaluated using:

**F1 Score**

F1 score balances precision and recall and is suitable for classification tasks where class imbalance may exist.

---

## Project Structure

```
ML_alrIEEEna_abhai
│
├── model.ipynb      # Complete notebook with EDA and model training
├── FINAL.csv        # Model predictions for TEST.csv
└── README.md        # Project documentation
```

---

## Output Format

The final submission file **FINAL.csv** contains:

| ID | CLASS |
| -- | ----- |
| 1  | 0     |
| 2  | 1     |
| 3  | 0     |

Where:

* **ID** → Test sample identifier
* **CLASS** → Model prediction (0 = Normal, 1 = Faulty)

---

## Tools & Libraries

The project was implemented using:

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* XGBoost

---

## Author

**Abhay Singh**

Machine Learning & Data Science Enthusiast
LinkedIn: https://www.linkedin.com/in/abhaysinghuk/
