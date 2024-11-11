# 📊 University Student Mental Health Analysis 🧠

Welcome to the **University Student Mental Health Analysis** project! This personal project explores university student mental health factors through data analysis and machine learning models. The goal is to gain insights into mental health patterns, especially focusing on changes pre- and post-COVID-19.


## 📜 Project Overview

Mental health is a critical area of study, especially among university students who often face unique pressures. This project analyzes a dataset from a survey conducted at the University of Victoria, Canada, examining various dimensions of student mental health such as depression, anxiety, mindfulness, and stress levels. 

Using machine learning, the project aims to predict mental health status based on lifestyle and demographic data, comparing pre- and post-COVID-19 stress levels to assess the pandemic's impact on students.

## 📁 Project Files

 The Jupyter Notebook containing all code for data processing, exploratory data analysis, model training, and evaluation.


## 🛠️ Key Steps and Methodology

### 1. Data Collection 📥

The dataset was sourced from the Borealis Database Repository. It consists of survey responses from university students, covering:
   - Demographic information (age, ethnicity, gender, etc.)
   - Lifestyle habits (exercise, sleep, mindfulness activities)
   - Mental health metrics (anxiety, depression, perceived stress scale)

### 2. Data Preprocessing 🧹

To ensure robust analysis, we preprocessed the data by:
   - **Cleaning**: Removing irrelevant and missing data entries.
   - **Feature Extraction**: Aggregating questions into composite scores for scales like CAMS (mindfulness), DASS (depression, anxiety, stress), and others.
   - **Feature Selection**: Selecting the most significant features using statistical tests, ultimately reducing the dataset to 17 key variables.

### 3. Exploratory Data Analysis (EDA) 📊

EDA was conducted to uncover initial patterns and relationships:
   - **Descriptive Statistics**: Summarized key statistics across variables.
   - **Visualizations**: Used box plots, histograms, and bar charts to display distributions of variables like age, mental health diagnosis, and perceived stress levels.

### 4. Machine Learning Models 🧠

Three classification models were tested to predict mental health status:
   - **K-Nearest Neighbors (K-NN)**: Implemented with Euclidean and Manhattan distances. After hyperparameter tuning, it achieved moderate accuracy but had a higher false negative rate.
   - **Decision Tree** 🌳: Built with pre- and post-pruning to avoid overfitting. Despite improvements, it still lagged behind Random Forest in predictive power.
   - **Random Forest** 🌲: This ensemble model provided the highest accuracy, precision, and recall, making it the most effective model for this analysis.

### 5. Model Evaluation 🧮

Each model was evaluated using the following metrics:
   - **Accuracy**: Percentage of correct predictions.
   - **Precision & Recall**: Measured to understand false positive and negative rates.
   - **F1 Score**: Indicates the balance between precision and recall.
   - **ROC-AUC Curve**: Demonstrates each model’s ability to distinguish between classes. The Random Forest model had the highest AUC score, confirming it as the best performer.

### 6. Statistical Testing (T-test) 📈

I used T-tests to compare pre- and post-COVID-19 stress levels using the Perceived Stress Scale (PSS). Results showed a statistically significant increase in stress post-COVID, indicating the pandemic’s impact on student mental health.

## 📈 Results & Conclusions

- **Best Model**: Random Forest achieved the highest accuracy (77.58%) with high precision (78%) and recall (95%).
- **Key Insights**: Significant predictors of mental health include disability status, mindfulness activities, and depression levels. Students who engage in mindfulness activities had better mental health outcomes.
- **COVID-19 Impact**: Statistical analysis confirmed a substantial rise in stress levels post-COVID-19.

## 📊 Visualizations

Visualizations used in the analysis include:
   - **Box Plots**: For identifying outliers in age and other continuous variables.
   - **Histograms and Bar Charts**: For categorical distributions, like mental health diagnoses by demographics.
   - **ROC Curves**: For model comparison.

## 🔧 Technologies & Libraries

- **Python** 🐍: Core language used for data manipulation and machine learning.
- **Libraries**:
   - `pandas` & `numpy`: For data preprocessing.
   - `matplotlib` & `seaborn`: For data visualization.
   - `scikit-learn`: For machine learning models and evaluation metrics.


