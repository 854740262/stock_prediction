# Stock Prediction

Build and test statistical model for stock prediction.
  
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/854740262/stock_prediction/master?filepath=https%3A%2F%2Fgithub.com%2F854740262%2Fstock_prediction%2Fblob%2Fmaster%2FProject.ipynb)
### Team member

  - Le Qin

### Problems/Motivation

-	The only question is, can people make money on stocks, without any finance related knowledge?
-	Model and test if predicting stock price in a short term(5-10 days) is viable
-	Model and test if predicting stock price in a long term(1-2 month) is viable

### What libraries/tools you will need. What you already know and what else you need to evaluate
-	Pandas
-	Numpy
-	Scikit-learn
-	Requests
-	Matplotlib 
-	fix-yahoo-finance: a python library, that scraps data from yahoo finance.
-	Stocks are full of risk and uncertainty. In order to make more accurate models, there are plenty of tools to use: TensorFlow, Keras.

### Data Collection details
- AMEX, NYSE, NASDAQ stock histories
    - https://www.kaggle.com/qks1lver/amex-nyse-nasdaq-stock-histories
    - Contains about 8000 stocks’ daily volume, open, close, high and low values since publicly listed.
- Data from yahoo finance
    - https://finance.yahoo.com/ 
    - Use for source of other data if they are not in the above collection.

### Any Literature review
- *A Machine Learning Model for Stock Market Prediction* by Osman Hegazy, Omar S. Soliman and Mustafa Abdul Salam. https://www.researchgate.net/publication/259240183_A_Machine_Learning_Model_for_Stock_Market_Prediction 
- *Stock Market Prediction Using Artificial Neural Networks* by Birgul Kutlu, Meltem Özturan and Bertan Badur. https://www.researchgate.net/publication/228407623_Stock_Market_Prediction_Using_Artificial_Neural_Networks 

### Required work detail before build model(clean up, hypothesis, data bias analysis etc.)
- The data collection is separated for each public listed company. To analysis the data, we must read and extract necessary information from them.
- There are few missing values in the data collection. To handle the missing values, the preferred way is using sk-learn and pandas to generate appropriate values.

### What is the predictive task and model detail. Model evaluation and selection strategy
- The task is predicting the stock prices for difference company and time periods.
- We will split data chronologically into training, validation and testing data. Model will be tuned and evaluated by the validation score of residuals. 

### How a user is going to test the final model. is there any webpage/command line interface. It can be like using curl from command line and calling a function(lambda via API gateway) in the cloud(AWS)
- For now, the user can test the final model on the testing set. As we haven’t covered the lambda via API gateway on class, the testing methods may vary.

### Tentative time line of activities



| Weeks | Tasks |
| ------ | ------ |
| 4-5 | Research and learn statistics and finance models |
| 6 | Data import and cleaning |
| 7-9 | Implement and validate different models |
| 10 | Write report and prepare presentation |



