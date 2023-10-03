# Financial_Analysis

Project Title:

Predicting Profit and Loss Using Logistic Regression

Problem Statement:

Predict whether a business transaction results in profit or loss based on cost of good sold and sale price.

Introduction:

In this project, we aim to predict whether a business transaction results in profit or loss using logistic regression. We'll utilize a dataset that includes key variables such as manufacturing price, sale price, gross sales, and discounts. The objective is to build a robust predictive model that helps classify transactions as profitable or not based on these financial metrics.

Dataset:

The dataset consists of the following columns:

'Manufacturing Price'
'Sale Price'
'Gross Sales'
'Discounts'
'Sales'
'COGS'
'Profit'
'PROFIT_LOSS'
Tools and Statistical Methods:

Programming Language: 
Python
Environment: Google Colab
Libraries: NumPy, Matplotlib, Seaborn, Pandas, Statsmodels, Scikit-Learn

Data Exploration and Insights:

In this section, we explore the dataset to gain insights into its characteristics.

Data Overview:

We begin by loading the dataset and examining its structure, including the column names and data types.

Descriptive Statistics:

We calculate summary statistics, such as mean, minimum, maximum, and standard deviation, for the dataset's numeric variables. This provides an initial understanding of the data distribution.

Here are some key statistics for the dataset:

Manufacturing Price Mean: 96.48
Sale Price Mean: 118.43
Gross Sales Mean: 182,759.40
Sales Mean: 169,609.06
COGS Mean: 145,475.21
Profit Mean: 24,133.87

It's important to note that the standard deviation for 'Sales' and 'COGS' is relatively high, indicating significant variance in the data.

Data Distribution: There is an imbalance in the dataset:

Profit Count: 642

Loss Count: 58

![Screenshot 2023-10-03 at 2 43 16 PM](https://github.com/Shalin96/Financial_Analysis/assets/139086441/d30aa9ac-52c3-4b12-8a17-1cc7883185d9)


The majority of transactions are classified as profit, which may affect the model's performance.

Correlation Analysis: 

We performed correlation analysis to assess the relationships between variables. A noteworthy finding is that 'Sales' has a strong positive correlation of 80% with 'Profit'. This suggests that 'Sales' is a major factor affecting profit.

![Screenshot 2023-10-03 at 2 44 22 PM](https://github.com/Shalin96/Financial_Analysis/assets/139086441/4dd2ffd9-3118-4f1b-9106-d925fc4fc868)


Logistic Regression Modeling:

The project proceeds with logistic regression, a statistical technique for binary classification.

Data Split:

The dataset is divided into training and testing sets, with 80% of the data used for training and 20% for testing the model.

Logistic Regression Model: 

We apply logistic regression to predict profit and loss based on the cost of good sold and sale price.

Model Evaluation: 

The model's performance is assessed using metrics such as accuracy. It's important to note that the model achieved an accuracy score of 100%, indicating its ability to classify transactions correctly. However, this high accuracy may be influenced by the dataset's imbalance and high standard deviation.

Overfitting:


One significant concern is that the model is overfitting the data. Overfitting occurs when a model learns the training data too well, including noise and random fluctuations, which can lead to poor generalization to new data. The reasons for overfitting in this model may include the dataset's imbalance, where there are 642 instances of profit and only 58 instances of loss. This class imbalance can cause the model to be biased towards the majority class, leading to an artificially high accuracy score. Additionally, the dataset exhibits high variance, particularly in the 'Sales' and 'COGS' variables, which can contribute to overfitting. These issues should be addressed to improve the model's reliability.


Conclusion:


In conclusion, the logistic regression model effectively predicts whether a business transaction results in profit or loss based on manufacturing price and sale price. The model demonstrates high accuracy, making it a valuable tool for decision-making and financial analysis. However, the findings suggest potential issues with data distribution, variance, and overfitting, which should be further investigated.

Future Work:


Future work may involve addressing the dataset's imbalance, reducing variance, and implementing techniques to mitigate overfitting. Additionally, the model can be extended to consider other factors that may impact profit and loss.
