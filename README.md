# Project Name: ML_Regression_Analysis
This project is a part of Supervised Machine Learning as well as my first Machine Learning project. I conducted this Regression Analysis on House Price data set. Both Simple and Multiple Linear Regression models are covered here.


## Supervised Machine Learning

The term 'Supervise' means to observe and direct the execution of a task, project or activity. In this type of Machine Learning the Client( The coder or data Scientist) supervise the model by teaching so that it can predict unknown or future instances. We teach the model by using training data. One thing to remember that the training data must be labeled. In this case, column names are called attributes, columns are called features.

## Regression

It is a supervised Machine Learning process of predicting continuous value (called as response or target, denoted by **Y**) using one or more continuous or categorical independent values (called as predictors or features, denoted by **X**). There are two types of Regression approaches. Simple Regression(Linear or Non-linear) and Multiple Regression(Linear or Non-linear).   Now let us consider an example. Suppose, we have a data set that contains house prices of 10 houses. First 9 house prices are given and they have a relation with the other attributes of the data set. By Regression Analysis, we can easily estimate the price of the last house by building a model.

## Regression Algorithms

To perform this Regression Analysis , there are many algorithms we can follow. They are all good algorithms, but all of them are not used in real life applications. The algorithms are - 
1. Ordinal Regression Analysis
2. Poisson Regression
3. Fast Forest Quantile Regression
4. Linear, polynomial, Lasso, Stepwise, Ridge Regularization
5. Bayesian Linear Regression
6. Neural Network Regression
7. Decision Forest Regression
8. Boosted Decision Tree Regression
10. KNN or K-Nearest Neighbours


## About the SaratogaHouses Data set

The data set is also attached in the file section of this project. This data set is easily available in GitHub as well as in Kaggle. This data set named **SaratogaHouses** has 1728 rows/observations and 16 columns/features/attributes/values. Generally the **price** column is considered as the **Response Variable**. The other columns can be considered as predictor variables. Observe that column **price** is a continuous column and other column are of mixed type. 

## Project Stages

Here I gone through some steps or stages to complete this project. In this project I build both Simple and Multiple Linaer Regression Model using the **sklearn** library and it's different modules. Here are detailed stages of this project.

**1. Basic Data Exploration:**

In this step, I read the data set using pandas read_csv() function in a variable called df. I then perform basic data exploration steps such as finding the shape, the column names and column types. I check all the codes working properly by using .head() method on the data frame df. After this to get a statistical summary of the numerical data in the data frame df , I use the .describe() method.

**2. Creating the Project Data Set:**

Here, I didn't consider the whole data set to malke the model. I only use the columns **price**, **livingArea**, **bedrooms**, **rooms** and **age**. I saved this short data in a variable called **reg**.

**3. Plotting the data:**

Here, firstly I used a histogram to show the distribution of data that are in the reg data frame. Then I plot a scatter plot of age, bedrooms,rooms and age against price to see if there exists any linear relationship. It is evident that in all cases, we can't pedict the relationship by just seeing the scatter plot.

**4. Train-Test Split:**

Now, the basic idea of this project is to build a model and train it with the train set (80% of the data) and use test set (20% of data) to check the model accuracy using different evaluation metrics. After that I plot the graph for train and test set to see whether there exists any different trend than normal data set plotting.

**5. Simple Linear Regression Model and Predicting with Model Evaluatio Metrics:**

Now, I build a Simple Linear Regression Model using **price** as response and **livingArea** as predictor. After building the model, I get the model intercept and the model coefficeint. One thing to remember that **np.asanyarray()** function is used to convert  data frame to an array as sklearn works only on array. After building and getting the model, I plotted them using scatter plot and line plot. The line we get is the best fit line of the model, also called as Regression Line. This line estiomates the error of the models as much small as possible. 


In the next step, I use the test set to predict the model outcomes (unknown house price) and define the model evaluationb metrics such as MAE (Mean Absolute Error), MSE (Mean Standard Error), R-Squared statistics , RSS (Residual Sum of Squares) etc.

**. Multiple Linear Regression Model and Predicting with Model Evaluation Metrics:**
















