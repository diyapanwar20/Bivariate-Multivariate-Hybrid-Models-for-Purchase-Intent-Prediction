# Bivariate-Multivariate-Hybrid-Models-for-Purchase-Intent-Prediction
E-commerce purchase intent prediction using hybrid bivariate and multivariate machine learning models

#  Purchase Intent Prediction using Bivariate–Multivariate Hybrid Models

##  Project Overview

Predicting whether an online visitor will make a purchase is a critical problem for e-commerce platforms. This project develops a **hybrid machine learning framework** that combines **bivariate behavioral signals** with **multivariate interaction patterns** to accurately predict customer purchase intent.

The system analyzes clickstream behavior such as product page visits, session duration, bounce rates, and traffic sources to determine the likelihood of purchase.

The final model integrates multiple machine learning and deep learning approaches to achieve **high predictive performance and strong generalization on imbalanced data**.



#  Business Objective

Most online visitors browse products but do not complete purchases. Accurately predicting **high-intent buyers** enables companies to:

• Improve product recommendations
• Increase conversion rates
• Optimize marketing campaigns
• Reduce unnecessary advertising costs
• Personalize the customer experience

This project builds predictive models to classify whether a session will generate **Revenue (Purchase)** or **No Purchase**.



#  Dataset Information

**Dataset:** Online Shoppers Purchasing Intention Dataset

**Total Sessions:** 12,330

**Total Features:** 18 behavioral attributes

**Target Variable:** Revenue

| Value | Meaning           |
| ----- | ----------------- |
| True  | Purchase occurred |
| False | No purchase       |

The dataset captures **real user clickstream behavior** on an e-commerce website.



#  Feature Categories

## Bivariate Behavioral Features

These features have a **direct relationship with purchase behavior**.

• ProductRelated
• ProductRelated_Duration
• PageValues

These features help identify **strong purchase signals**.



## Multivariate Behavioral Features

These features interact with other variables to reveal **complex purchase patterns**.

Examples:

• BounceRates
• ExitRates
• Month
• VisitorType
• TrafficType
• Region
• Browser
• OperatingSystems
• Weekend

Multivariate modeling captures **hidden interactions between user behaviors**.



# Technologies Used

**Programming Language**

• Python

**Data Analysis**

• Pandas
• NumPy

**Visualization**

• Matplotlib
• Seaborn

**Machine Learning**

• Scikit-Learn
• XGBoost
• Imbalanced-Learn (SMOTE)

**Deep Learning**

• TensorFlow
• Keras

**Other Tools**

• PCA (Dimensionality Reduction)
• Feature Selection (Chi-Square Test)

---

#  Project Workflow

1️) Data Loading and Inspection

2️) Data Preprocessing
• Handling categorical variables
• Boolean encoding
• Feature preparation

3️) Exploratory Data Analysis (EDA)
• Target distribution
• Correlation analysis
• Behavioral insights

4️) Feature Engineering

5️) Feature Selection using Chi-Square

6️) Dimensionality Reduction using PCA

7️) Handling Imbalanced Data using SMOTE

8️) Model Training

9️) Hyperparameter Optimization using GridSearchCV

10)  Hybrid Model Construction

1️) Deep Learning Models

2️) Model Evaluation and Comparison



#  Machine Learning Models Implemented

Traditional models were trained using both **bivariate and multivariate feature sets**.

• Logistic Regression
• Decision Tree
• Random Forest
• AdaBoost
• Naive Bayes
• K-Nearest Neighbors
• Support Vector Machine
• XGBoost

Each model was evaluated using multiple performance metrics.



#  Deep Learning Models

## Artificial Neural Network (ANN)

A deep neural network was trained on **multivariate PCA features** to capture complex nonlinear behavioral patterns.

Architecture includes:

• Dense layers
• Dropout for regularization
• Sigmoid output for binary classification

---

## DeepFM Hybrid Model

DeepFM combines two components:

**Factorization Machine Component**

Captures feature interactions among behavioral variables.

**Deep Neural Network Component**

Learns high-order nonlinear relationships between user behavior patterns.

This model is widely used in **recommendation systems and advertising prediction systems**.

---

#  Hybrid Machine Learning Model

The final system combines:

• **Tuned Bivariate XGBoost Model**
• **Tuned Multivariate XGBoost Model**

Using a **Soft Voting Ensemble Classifier**.

### Why Hybrid?

Bivariate model captures **strong behavioral signals**
Multivariate model captures **complex interaction patterns**

Combining both improves **model robustness and predictive performance**.

---

#  Model Evaluation Metrics

Models were evaluated using the following metrics:

• Accuracy
• Precision
• Recall
• F1 Score
• ROC-AUC Score

For imbalanced datasets, **ROC-AUC and Recall** are the most important indicators.

---

#  Best Model Performance

**Final Model:** Hybrid_XGB_Voting

Performance Results:

| Metric   | Score    |
| -------- | -------- |
| Accuracy | High     |
| Recall   | ~75%     |
| F1 Score | Strong   |
| ROC-AUC  | **0.91** |

The hybrid model achieved the **highest discrimination ability** for identifying potential buyers.

---

#  Key Insights

• Multivariate models outperform simple bivariate models

• Ensemble models provide better generalization

• Hybrid models improve prediction stability

• Deep learning models capture complex user behavior patterns

• The Hybrid XGBoost Voting model achieved the **best overall performance**

---

#  Business Impact

This predictive system can help e-commerce companies:

*  Identify high-intent customers

*  Personalize marketing campaigns

*  Improve product recommendation systems

*  Increase sales conversion rates

* Optimize digital advertising strategies



#  Future Improvements

• Deploy the model using FastAPI or Flask

• Build a real-time prediction API

• Implement automated feature engineering

• Integrate with recommendation systems

• Apply advanced deep learning architectures











**Diya Panwar**

Data Science | Machine Learning | Deep Learning

Passionate about building intelligent systems that transform data into actionable insights.
