# LinerRegressionFromScratch

## Project Description:

This project focuses on predicting stock prices using a **univariate linear regression algorithm**, built entirely from scratch without the use of any machine learning libraries such as Scikit-learn or TensorFlow. The goal of this project is twofold:

1. **To predict stocks' future closing prices** based on historical closing price data.
2. **To gain a deep understanding of how the linear regression algorithm works** by implementing every aspect manually, from the cost function to the optimization process.

### Key Aspects of the Project:

1. **Data Collection and Preprocessing**:
   - **Historical Stock Data**: The dataset consists of daily historical closing prices of a selected stock. The data is cleaned to remove any null values.
   - **Feature and Label**: In this univariate regression model, the only feature is the stocks' closing price on the previous day, and the label is the stocks' closing price on the given day.
   - **Feature extraction**: Feature is extracted by using the close price of the previous day for predicting the close price of the next day.

2. **Algorithm Explanation**:
   - **Univariate Linear Regression**: The model aims to find a linear relationship between the previous day closing price and a given close price for a stock. The relationship is modeled using the linear equation:
     - \( y = wx + b \)
     - Where \( y \) is the predicted current closing stock price, \( x \) is the previous day close price, \( w \) is the slope of the line, and \( b \) is the intercept.
   - The algorithm works by iteratively adjusting the values of \( w \) and \( b \) to minimize the **mean squared error (MSE)** between predicted and actual stock prices, using **gradient descent** as the optimization technique.

3. **Understanding Linear Regression**:
   - The primary goal of this project is **to learn how the linear regression algorithm works**. By manually coding the process, the project provides hands-on experience in:
     - **Calculating the cost function (MSE)**.
     - **Deriving the gradient** of the cost function to understand how changes in the slope and intercept affect predictions.
     - **Applying gradient descent** to iteratively update the slope and intercept until the cost function reaches its minimum.
   - This approach ensures a comprehensive understanding of the underlying mathematical concepts and mechanics of linear regression.

4. **Model Building**:
   - **Initialization**: The slope (\(w\)) and intercept (\(b\)) are initialized randomly.
   - **Cost Function**: MSE is used to measure the difference between actual and predicted stock prices.
   - **Gradient Descent**: Updates the parameters (slope and intercept) to reduce the error in predictions.
   - **Convergence**: The model stops training once the cost function reaches a minimal value or the changes in the parameters become sufficiently small.

5. **Model Training and Testing**:
   - The data is divided into training and testing sets. The linear regression model is trained on the historical stock data in the training set to learn the relationship between time and stock price.
   - Once trained, the model is tested on the unseen test data to evaluate its performance.

6. **Evaluation Metrics**:
   - The model is evaluated using **Root Mean Squared Error (RMSE)**, providing insight into the accuracy of the predicted stock prices compared to actual stock prices.

7. **Visualization**:
   - A comparison plot of how well does the **linear regression model** represents the **training data** is provided.
   - A comparison plot of **actual vs predicted stock prices** is generated to visually inspect how closely the predictions align with the real data.
   - A **loss curve** is created to visualize the reduction in the cost function over iterations, showing how the model improves during training.

## Objectives:
- Build a univariate linear regression model from scratch to predict stock prices.
- **Deeply understand the inner workings of linear regression**, including gradient descent, parameter updates, and error minimization.
- Explore how historical stock price data can be used to predict future trends.
- Visualize the model’s performance and track its learning process.
