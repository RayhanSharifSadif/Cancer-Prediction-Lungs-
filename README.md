# Lung Cancer Prediction

Lung Cancer Prediction achieved using the `sklearn` library for the CSE422 course at <a href="https://www.bracu.ac.bd/">BRAC University</a>.

## Overview

This project focuses on predicting lung cancer using machine learning techniques. The dataset utilized for this project is sourced from [Kaggle](https://www.kaggle.com/datasets/rishidamarla/cancer-patients-data). As part of the data preprocessing process, null values were introduced into the dataset using the script shown below to demonstrate how to handle them.

![Inserting Null Values Script](https://github.com/ShakeefAhmedRakin/LungCancerPrediction/assets/112527326/67d3e30f-1bd1-469d-bd29-c6686f5928a1)

## Data Preprocessing

The following steps were taken during data preprocessing:

- Duplicate columns like **"Smoking"** and **"Swallowing Difficulty"** were removed.
- Columns like **"Patient id"** which do not contribute to the results were dropped.
- Missing values were handled through imputation using the "SimpleImputer" from `sklearn`. The mean strategy was employed.
- Categorical features like **"Gender"** and **"Level"** were encoded with appropriate values.
- Less informative features, such as **"Genetic Risk"** and **"Occupational Hazard"**, were dropped using correlation analysis, visualized using Seaborn.
- The dataset was divided into training (75%) and test (25%) sets, with two variants for each: one scaled using "MinMaxScaler" and the other unscaled.

## Model Evaluation

Both scaled and unscaled variants of the training and test sets were used to evaluate various machine learning models:

- Decision Tree
- Naive Bayes
- Random Forest
- Support Vector Machine
- Grid Search
- KNeighborsClassifier
  
## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/ShakeefAhmedRakin/LungCancerPrediction.git
   ```

2. Install the required dependencies:

   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn
   ```

3. Run the provided Python script.

## The Code

![Project Code](https://github.com/ShakeefAhmedRakin/LungCancerPrediction/assets/112527326/ca470da5-8419-428e-b957-5e65f2e21b74)
