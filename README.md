# Cardiovascular Risk Assessment

In this project, I developed a binary classification model by systematically assessing the original dataset, iterative preprocessing, model performance validation and improvements using hyperparameter tuning methods such as Bayesian and Optuna optimizations and exploring the importance of threshold optimization. Meaningful EDA was performed by understanding the interactions between the predictors through visualizations such as histograms, scatterplots, etc. The data preprocessing steps where streamlined through data pipelines considering the multiple preprocessing techniques used for developing the final model. The model performance where guaged mainly by the AUC metric whose value was increased by 7% from the baseline, enhancing the predictions made by the model.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [License](#license)


## Introduction

This project aims to build an accurate classification model for assessing cardiovascular risk based on a range of health and lifestyle features. Key steps in the project include:

Domain-Relevant Data Wrangling: Emphasized dataset attribute interactions to ensure meaningful analysis.
Exploratory Data Analysis (EDA): Conducted detailed EDA to evaluate feature variability, which is crucial for accurate classification predictions.
Data Pre-Processing: Implemented streamlined data preprocessing techniques using pipelines with appropriate transformations. Iteratively validated the reliability of these techniques across multiple models.
Model Optimization: Enhanced model performance by optimizing using AUC and achieving a 7% improvement in overall accuracy.


## Installation

1. Clone the repository:
git clone https://github.com/BHARATH-V-P/Cardiovascular-Risk-Assessment
2.  to the project directory:
cd Cardiovascular-Risk-Assessment
3. Install dependencies:
pip install -r requirements.txt

## Usage
1. Prepare Your Dataset: Place your datasets in the data/ directory. Ensure the dataset is named cardiovascular_data.csv or adjust the script accordingly.
2. Open the Jupyter Notebook:
jupyter notebook "HEART_ EDA _CONCISE_final.ipynb"
3. The script will:
- Data Preprocessing: Handles missing values, duplicate values, normalization and encoding of all predictors as needed.
- Perform detailed EDA to understand feature impacts on cardiovascular risk.
- Implement feature engineering and feature selection using data pipelines.
- Perform Bayesian Optimization on selected models based on initial model validations
- Optimize model performance and validate results using AUC and accuracy.
- Explore the importanc eof threshold optimization for a binary classification problem and understanding the extent of its overall impact.
- 
## Features
   
- Preprocess the raw data though data cleaning and data exploration.
- Apply neccessary normalization and transformations to features.
- Exploratory Data Analysis: Provides insights into feature variability and interactions with one another and the target variable.
- Perform feature engineering based on results drawn from feature selection and feature transformations.
- Model Training: Utilizes different machine learning models to define baseline performances. Which helps in determining the models that could be potentially improved upon adopting strategies related to feature engineering and model hyperparameter optimization.
- Performance optimization- Bayesian Hyperparameter optimization on XGB Classifier and Random Forest Classifier models accross different configurations.
- Uses AUC and accuracy as evaluation metrics to develop an optimum objective for model improvement.
- Utilizing threshold importance to asses how models optimized based on optimum threshold compares with the base models.
  
## Results
### Baseline Model Performance
-----
I evaluated the performance of various classifiers across three different preprocessing methods. Key metrics such as Accuracy, Precision, F1 Score, Recall, and ROC AUC were used to assess the models.

**Preprocessing Method 1:** The SVC model achieved the highest performance with an accuracy of 90.2% and an ROC AUC of 0.948. Logistic Regression, Random Forest, and Gradient Boosting models all performed similarly with accuracies of around 85.2% and ROC AUC scores ranging from 0.914 to 0.937.

**Preprocessing Method 2:** Logistic Regression and SVC both demonstrated strong performance with accuracies of 88.5% and ROC AUCs of approximately 0.947 and 0.953, respectively. The Random Forest classifier also performed well with an accuracy of 86.9% and an ROC AUC of 0.947. GaussianNB had a notable drop in performance with an accuracy of 72.1% and an ROC AUC of 0.893.

**Preprocessing Method 3:** The GaussianNB and Random Forest classifiers achieved the highest accuracy of 90.2%, with ROC AUCs of 0.917 and 0.932, respectively. SVC also performed well with an accuracy of 90.2% and an ROC AUC of 0.950. Logistic Regression and Quadratic Discriminant Analysis both achieved an accuracy of 88.5% with ROC AUCs close to 0.941 and 0.919, respectively.

### Model Optimization
-----
To further enhance model performance, I applied Bayesian Hyperparameter optimization to the XGBoost and Random Forest classifiers.

**XGBoost:** The best-performing configuration was achieved using direct accuracy optimization, resulting in an accuracy of 93.4% and an F1 score of 0.938. The ROC AUC for this model was 0.909. Other optimized configurations also yielded strong results, with accuracy scores ranging from 85.2% to 91.8% and ROC AUCs reaching up to 0.965.

**Random Forest:** The best results were obtained through direct accuracy optimization, which resulted in an accuracy of 90.2%, an F1 score of 0.903, and an ROC AUC of 0.935. Other configurations yielded similar performance, with accuracy scores around 88.5% to 90.2% and ROC AUCs up to 0.948.

### Threshold Optimization
-----
For each model, I optimized the decision threshold to maximize the ROC AUC. SVC performed the best with an optimized ROC AUC of 0.950 at a threshold of 0.493. Logistic Regression and Random Forest models also showed strong ROC AUC values of 0.941 and 0.932, respectively, with thresholds around 0.52.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
