# Anemia Detection Using TabNet

An AI-based anemia classification project using **TabNet**, **SABO-based feature selection**, and **GWCA-based hyperparameter optimization**.

## Project Overview

This project develops a machine learning model for anemia detection from medical dataset features.

The workflow includes:

1. Data preprocessing
2. Missing-value handling
3. Feature selection using SABO-based ranking
4. Hyperparameter optimization using GWCA
5. TabNet classification
6. 3-fold stratified cross-validation
7. Confusion matrix and accuracy evaluation

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* PyTorch
* PyTorch TabNet
* Matplotlib
* Seaborn

## Machine Learning Methods

### SABO Feature Selection

SABO-based feature ranking is used to identify the most important features for anemia classification.

The project selects the top features based on their calculated ranking scores.

### GWCA Hyperparameter Optimization

GWCA is used to search for suitable TabNet hyperparameters, including:

* `n_d`
* `n_a`
* `n_steps`
* `lambda_sparse`
* Learning rate

The candidate configurations are evaluated using stratified cross-validation.

### TabNet Classification

The selected features are used to train a **TabNet Classifier** for anemia classification.

The model uses:

* Adam optimizer
* Configurable learning rate
* Early stopping
* Cross-validation

## Model Evaluation

The project evaluates the model using:

* Accuracy
* Confusion Matrix
* 3-Fold Stratified Cross-Validation
* Feature ranking visualization

## Project Structure

```text
Anemia-detection-tabnet/
│
├── anemia_detection_tabnet.py
├── requirements.txt
├── README.md
└── .gitignore
```

## Installation

Clone the repository:

```bash
git clone https://github.com/keerthana-n15/Anemia-detection-tabnet.git
cd Anemia-detection-tabnet
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

## Dataset

The Python program expects a CSV dataset named:

```text
anemia.csv
```

Place the dataset in the project directory before running the program.

## Running the Project

Run:

```bash
python anemia_detection_tabnet.py
```

## Results

The project generates feature-ranking and confusion-matrix visualizations and evaluates the model using stratified cross-validation.


