## Linear Regression Analysis

### I. Introduction

Linear Regression is a straightforward yet powerful statistical method used for predicting a dependent variable based on one or more independent variables. It is particularly useful for understanding the relationships between variables and making predictions.

### II. Steps

#### a) Data Preprocessing

To ensure the accuracy and reliability of our model, the following preprocessing steps were undertaken:

- **Standardization of Features**: Standardization was applied to normalize the features, ensuring each feature contributes equally to the model.
- **Handling Missing Values**: Any missing values were handled through appropriate techniques to maintain data integrity.

#### b) Features & Target

- **Features**:
- 
  - Net Sales Lag 1
  - Net Sales Growth
  - Net Sales Lag 2
  - Net Sales Growth 2
    
- **Target**: 12 Months Ended (Net Sales)

#### c) Model Training

The model was trained using the training dataset, fitting the model to the data to capture the underlying patterns and relationships.

#### d) Hyperparameters

The Linear Regression model was trained with default settings, which include:

- **fit_intercept**: True
- **normalize**: False (standardization was performed manually)

#### e) Performance Metrics

The performance of the Linear Regression model was evaluated using the following metrics:

- **Mean Absolute Error (MAE)**: 17098.37
- **Root Mean Squared Error (RMSE)**: 17306.38
  
The performance of the Linear Regression model was evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). The MAE of 17098.37 represents the average absolute difference between the predicted and actual values of Net Sales, indicating the typical prediction error in millions of dollars. The RMSE of 17306.38 measures the square root of the average squared differences between predicted and actual values, providing a measure of the model's prediction accuracy with a greater emphasis on larger errors. In the context of our project, these metrics reflect the model's effectiveness in predicting Home Depot's quarterly revenue, with lower values indicating better predictive performance and closer alignment with actual sales figures.

#### f) Interpretation

The model provides the following insights:

- **Intercept**: 1748.36
- **Coefficients**:
  - **Net Sales Lag 1**: 0.27
  - **Net Sales Growth**: 25.69
  - **Net Sales Lag 2**: 0.26
  - **Net Sales Growth 2**: 1008.08
 
  The intercept value of 1748.36 in the Linear Regression model represents the baseline level of Net Sales when all other independent variables are zero. Essentially, this is the expected Net Sales in millions if there were no contributions from the factors such as Net Sales Lag 1, Net Sales Growth, Net Sales Lag 2, and Net Sales Growth 2.

The coefficient for Net Sales Lag 1 is 0.27, indicating that for each unit increase in the Net Sales from the previous quarter, the Net Sales in the current quarter are expected to increase by 0.27 million dollars, assuming all other factors remain constant. This demonstrates a modest positive influence of past sales on current sales. The coefficient for Net Sales Growth is 25.69, showing a strong positive relationship between the growth in Net Sales and the current quarter’s Net Sales. For each unit increase in the percentage growth of Net Sales, the current quarter’s Net Sales are expected to increase by 25.69 million dollars, highlighting the significant impact of sales growth on current sales figures.

Similarly, the coefficient for Net Sales Lag 2 is 0.26, suggesting that sales from two quarters ago positively affect the current quarter’s sales, albeit slightly less than the immediate previous quarter. The coefficient for Net Sales Growth 2 is 1008.08, indicating a substantial impact of the growth in sales from two quarters ago on the current quarter’s sales, emphasizing that past growth trends play a critical role in determining current sales performance. Overall, these coefficients provide valuable insights into how

 #### g) Conlcusion
 
The Linear Regression model was selected due to its superior performance metrics compared to other models. It effectively captures the relationships between the features and the target variable, providing accurate predictions for Home Depot's quarterly revenue.

The Linear Regression model's ability to predict quarterly revenue with reasonable accuracy makes it a valuable tool for Home Depot's decision-making process. It assists in improving operational efficiency and maximizing profitability by providing data-driven insights.
