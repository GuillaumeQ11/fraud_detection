# Fraud Detection System

This project implements a **Fraud Detection System** using various machine learning models and techniques, including **Logistic Regression**, **Random Forest**, and **XGBoost**. The system is designed to detect fraudulent transactions in a banking dataset, with a strong focus on handling class imbalance using **SMOTE**.

## Table of Contents

- [Project Overview](#project-overview)
- [Installation](#installation)
- [Models Used](#models-used)
- [Data](#data)
- [Results](#results)
- [License](#license)
- [Author](#author)

## Project Overview

This project aims to build and evaluate a fraud detection model using **imbalanced datasets**, where the fraudulent transactions represent a very small percentage of the total transactions. Various machine learning algorithms are tested to determine the best approach for accurately detecting fraud.

### Key Features:
- **SMOTE** applied to balance the dataset.
- Evaluation using **AUC**, **Precision**, **Recall**, and **F1-score**.
- Comparison of **Logistic Regression**, **Random Forest**, and **XGBoost** models.

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fraud-detection.git
   cd fraud-detection

2. Create a virtual environment 
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows, use venv\Scripts\activate

3. Install the required dependecies
   ```bash
   pip install -r requirements.txt

## Models used
### Logistic Regression
A simple yet effective model for binary classification, widely used in fraud detection systems. It is evaluated with and without SMOTE to compare its performance.
### Random Forest
A robust ensemble learning model that has shown strong results in detecting fraud due to its ability to handle imbalanced datasets.
### XGBoost
An efficient gradient boosting model that typically performs well with imbalanced datasets. It is tested and compared with the other models for superior performance.

# Data
The data used for this project can be found here :
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Results

### Performance with SMOTE:

- **Random Forest** achieved the best results with an **AUC of 0.9800**, **precision of 0.86**, and **recall of 0.79** for the fraudulent class (1).
- **XGBoost** also showed strong performance with an **AUC of 0.9718**, **precision of 0.72**, and **recall of 0.80** for the fraudulent class.
- **Logistic Regression**, despite an **AUC of 0.9716**, had **low precision for the fraudulent class (0.06)** but a **high recall (0.88)**.

### Performance without SMOTE:

- **Random Forest** remains solid with an **AUC of 0.9267**, but with **precision of 0.91** and **recall of 0.75** for the fraudulent class.
- **XGBoost** had an **AUC of 0.9691**, with **precision of 0.95** an



## License

This project is licensed under the MIT License.

## Author
GuillaumeQ11 - [GitHub](https://github.com/GuillaumeQ11)