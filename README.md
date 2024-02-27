# Movie-Budget-Revenue-Analysis
This projecct analyzes movie data from The Numbers to better understand what types of movie have been the most successful in last decade 

## Project Overview
Simple linear regression project to model the relationship between movie budgets and their revenue

## 1. Introduction
In this project, I built a Linear Regression model to study the linear relationship between a movie's production budget and its worldwide revenue. I used the Python programming language with the relevant modules to analyse, clean and visualise the data.

## 2. Tools Used
* *JupyterLab* - A web-based interactive development environment for notebooks, data and code.
#### Python Modules
* *pandas* - Provided necessary tools to manipulate the data and clean the data.
* *matplotlib* - Used to create basic plots in Python.
* *scikit-learn* - Provides simple tools for effective and efficient data analysis applications.
* *seaborn* - It provides a high-level interface for drawing attractive and informative statistical graphics.

## 4. The Dataset
The dataset was scraped from "The Numbers" at https://www.the-numbers.com/movie/budgets/all 

## 5. Data Exploration, Visualisation and Analysis
I used *pandas* to read the CSV file using the standard read_csv() function into a DataFrame. I explored the data and discovered that there were a lot of null or zero values for movies which had either not come out yet or had incomplete data. I dropped all of such conflicting rows. <br/>
I then used matplotlib to plot a scatter diagram of the dependent variable - movie revenue against the independent variable - movie budget.

## 6. The Model
Simple linear regression is the simplest machine learning algorithm. Linear Regression is used to find the linear relationship between a target and one or more predictors/features.<br/>
Simple linear regression is used to check and find the relationship between one target and one feature. It detects statistical relationships that roughly predict the dependent variable (revenue) based on the independent variable (budget). <br/> 
I used the scikit-learn module to build a linear regression model using the data, generating a line of best fit. I obtained the slope to be 3.12259592. I then plotted this line of best fit on the scatter plot using matplotlib once more.

## 7. Evaluating the Model
I also used the scikit-learn module to obtain the goodness of fit score to be 0.55770, in other words, the linear regression model can accurately predict 55% of the revenue values based off the budget values using the regression model.

## 8. Conclusion
Based off the goodness of fit score, it is evident that the model is not good enough to deploy on new data. The budget alone cannot be accurately used to predict the revenue. We would need to consider other factors such as date of release, the production studio and whether or not the movie is a sequel. This would help to give a more accurate relationship and prediction of movie revenue.
