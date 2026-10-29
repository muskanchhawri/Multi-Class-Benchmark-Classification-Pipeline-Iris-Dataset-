# Multi-Class-Benchmark-Classification-Pipeline-Iris-Dataset-
Multi-class Iris flower classification using Logistic Regression and Decision Tree, with EDA, feature scaling, model evaluation, and performance comparison.

## Project Overview

This project implements a multi-class classification pipeline using the Iris dataset. It explores the dataset, performs data cleaning and feature scaling, trains two machine learning models, and compares their performance using standard evaluation metrics.

## Objectives

- Load and inspect the Iris dataset.
- Perform Exploratory Data Analysis (EDA).
- Handle duplicate records.
- Apply feature scaling using StandardScaler.
- Split the dataset into training and testing sets.
- Train and evaluate two classification algorithms.
- Compare model performance using evaluation metrics.
- Save trained models for future use.

## Dataset Information

The Iris dataset contains measurements of three flower species:

- Setosa
- Versicolor
- Virginica

**Features:**
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

**Target:** Species

| Property | Details |
|---|---|
| Original records | 150 |
| Features | 4 numerical columns |
| Target column | Species |
| Classes | 3 |
| Records after duplicate removal | 149 |

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

## Project Workflow

### 1. Data Loading and Inspection
Loaded the Iris dataset and examined its shape, column names, data types, summary statistics, missing values, and duplicate records.

### 2. Exploratory Data Analysis
Created visualizations to understand the dataset:
- Species distribution count plot
- Feature distribution histograms
- Pairplot for feature relationships
- Correlation heatmap
- Boxplots for potential outlier detection

### 3. Data Cleaning
Checked for missing values and removed one exact duplicate row.

### 4. Feature Scaling
Used StandardScaler within Scikit-learn pipelines to standardize features without leaking information from the test set into training.

### 5. Train-Test Split
Split the cleaned dataset into 80% training data and 20% testing data, using stratification to preserve class proportions.

### 6. Model Training
Trained two classification models:

- Logistic Regression
- Decision Tree Classifier

### 7. Model Evaluation
Evaluated the models using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 8. Model Comparison
Compared the performance of both models using a metrics table and an accuracy bar chart.

## Model Evaluation Results

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 0.933 | 0.933 | 0.933 | 0.933 |
| Decision Tree | 0.933 | 0.933 | 0.933 | 0.933 |

Both models achieved **93.3% accuracy** on the current test split. Their evaluation scores were equal in this experiment.

## Saved Models

The trained model pipelines are saved as:

- `logistic_regression_model.pkl`
- `decision_tree_model.pkl`

These files contain the trained pipelines, including preprocessing where applicable.

## How to Run the Project

1. Clone or download this repository.
2. Open the project folder in Jupyter Notebook.
3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn joblib jupyter
   ```

4. Open and run the project notebook from the first cell to the last.
5. Ensure the Iris dataset file is available if the notebook loads it from a CSV file.

## Conclusion

This project demonstrates a complete introductory multi-class classification workflow, from dataset inspection and exploratory analysis to preprocessing, model training, evaluation, comparison, and model saving.

Both Logistic Regression and Decision Tree achieved 93.3% accuracy on the current test set. Further testing with different splits or cross-validation could help assess how consistently the models perform.

## Author

**Muskan Chhawri**

## Project Name

**Datheon — Multi-Class Benchmark Classification Pipeline (Iris Dataset)**
