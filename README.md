# Anomaly Detection in Electrical Systems

A machine learning project that detects anomalies in electrical power grid systems using a Random Forest Classifier.

## Project Overview

This project analyzes electrical system data to identify anomalies and classify feeders by distribution company (DISCO). It uses supervised machine learning to train a model on historical power grid data and evaluates its performance using various metrics including accuracy, precision, recall, confusion matrix, and multiclass ROC curves.

## Project Structure
Anomaly-Detection-in-Electrical-Systems/
│
├── Anomaly_detection_in_electrical_systems.ipynb  # Main notebook
├── data.csv                                        # Dataset
├── requirements.txt                                # Python dependencies
├── .gitignore                                      # Git ignore rules
└── README.md                                       # Project documentation

## 🚀 Getting Started

### 1. Clone the Repository

### 2. Create and Activate Virtual Environment
```bash
python -m venv myenv

# Windows
myenv\Scripts\activate
```

### 3. Install Dependencies
```bash
python -m pip install -r requirements.txt
```

### 4. Run the Notebook
Open `Anomaly_detection_in_electrical_systems.ipynb` in Jupyter or VS Code and run all cells.

---

## Dataset

The dataset contains electrical power grid readings with the following key attributes:

- **Feeder Identifier** — unique ID for each feeder
- **Substation** — substation name
- **Feeder** — feeder name
- **discoName** — distribution company name (target variable)

## Machine Learning Pipeline

| Step | Details |
|------|---------|
| **Algorithm** | Random Forest Classifier |
| **Train/Test Split** | 80% / 20% |
| **Target Variable** | `discoName` |
| **Evaluation Metrics** | Accuracy, Precision, Recall, ROC-AUC |


## Model Evaluation

The model is evaluated using:

- **Accuracy Score** — overall correctness of predictions
- **Precision & Recall** — weighted average for multiclass
- **Confusion Matrix** — visualizes true vs predicted labels
- **Multiclass ROC Curve** — one curve per class using label binarization

## Tech Stack

- Python 3.10+
- pandas
- scikit-learn
- matplotlib
- seaborn
- joblib

## Requirements

See `requirements.txt` for full list of dependencies.
