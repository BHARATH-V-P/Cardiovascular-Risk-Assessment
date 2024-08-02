#Cardiovascular Risk Assessment

The Cardiovascular Risk Assessment project focuses on evaluating cardiovascular risk by analyzing various health metrics, lifestyle factors and more . The project involves a comprehensive approach to data wrangling, exploratory data analysis (EDA), and model optimization to accurately predict cardiovascular risk. 

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [License](#license)


##Introduction

This project aims to build an accurate classification model for assessing cardiovascular risk based on a range of health and lifestyle features. Key steps in the project include:

Domain-Relevant Data Wrangling: Emphasized dataset attribute interactions to ensure meaningful analysis.
Exploratory Data Analysis (EDA): Conducted detailed EDA to evaluate feature variability, which is crucial for accurate classification predictions.
Data Pre-Processing: Implemented streamlined data preprocessing techniques using pipelines with appropriate transformations. Iteratively validated the reliability of these techniques across multiple models.
Model Optimization: Enhanced model performance by optimizing using AUC and achieving a 7% improvement in overall accuracy.


##Installation

1. Clone the repository:
git clone https://github.com/yourusername/Cardiovascular-Risk-Assessment
2.  to the project directory:
cd Cardiovascular-Risk-Assessment
3. Install dependencies:
pip install -r requirements.txt

##Usage
1. Prepare Your Dataset: Place your datasets in the data/ directory. Ensure the dataset is named cardiovascular_data.csv or adjust the script accordingly.
2. Open the Jupyter Notebook:
jupyter notebook "Cardiovascular_Risk_Assessment_EDA.ipynb"
The script will:
- Preprocess the raw data, including checking for null values and duplicates.
- Perform detailed EDA to understand feature impacts on cardiovascular risk.
- Implement feature engineering and selection through pipelines.
- Optimize model performance and validate results using AUC.
- Review evaluation metrics and predictions.
- Features
- Data Preprocessing: Handles missing values and applies normalization and transformations.
- Exploratory Data Analysis: Provides insights into feature variability and interactions.
- Feature Engineering: Includes feature selection and transformation.
- Model Training: Utilizes various machine learning models for classification.
- Performance Optimization: Uses AUC for model performance evaluation and accuracy improvement.
3. Model Evaluation: Assesses model performance and accuracy through various metrics.
  
## Results
Data Wrangling and EDA: Detailed data wrangling and EDA ensured accurate feature interactions and variability assessment.
Pre-Processing Techniques: Streamlined preprocessing techniques were validated and optimized across multiple models.
Model Performance: Achieved a 7% improvement in overall model accuracy through iterative optimization and validation.
License
This project is licensed under the MIT License - see the LICENSE file for details.
