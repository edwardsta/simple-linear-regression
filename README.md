# Linear Regression with One Variable
This example was completed for the course 'Machine Learning' by Andrew Ng, Coursera (Adapted from Stanford CS229)

## Overview
In this exercise, we implement linear regression with one variable to predict proﬁts for a food truck. Suppose you are the CEO of a restaurant franchise and are considering diﬀerent cities for opening a new outlet. The chain already has trucks in various cities and you have data for proﬁts and populations from the cities.

You would like to use this data to help you select which city to expand to next. The ﬁle ex1data1.txt contains the dataset for our linear regression problem. The ﬁrst column is the population of a city and the second column is the proﬁt of a food truck in that city. A negative value for proﬁt indicates a loss. The ex1.m script has already been set up to load this data for you.

## Plotting the Data
Before starting on any task, it is often useful to understand the data by visualizing it. For this dataset, you can use a scatter plot to visualize the data, since it has only two properties to plot (proﬁt and population). (Many other problems that you will encounter in real life are multi-dimensional and can’t be plotted on a 2-d plot.) In ex1.m, the dataset is loaded from the data ﬁle into the variables X and y. Next, the script calls the plotData function to create a scatter plot of the data. When you run ex1.m, our end result should look like Figure 1, with the same red “x” markers and axis labels.

![alt text](https://github.com/edwardsta/simple-linear-regression/blob/master/Figure1.PNG)

## Gradient Descent
Now we implement gradient descent with the file gradientDescent.m. Make sure you understand what you are trying to optimize and what is being updated. Keep in mind that the cost J(θ) is parameterized by the vector θ, not X and y. That is, we minimize the value of J(θ) by changing the values of the vector θ, not by changing X or y.

A good way to verify that gradient descent is working correctly is to look at the value of J(θ) and check that it is decreasing with each step. The starter code for gradientDescent.m calls computeCost on every iteration and prints the cost. The value of J(θ) should never increase, and should converge to a steady value by the end of the algorithm.

Once this is performed, ex1.m will use the final parameters to plot the linear fit. The result should look something like Figure 2.

![alt text](https://github.com/edwardsta/simple-linear-regression/blob/master/Figure2.PNG)

## Visualizing the Cost Function J(θ)

The script ex1.m will produces a 2-D array of J(θ) which are used to create surface and contour plots of J(θ) using the surf and contour commands. The plots should look something like Figure 3.

![alt text](https://github.com/edwardsta/simple-linear-regression/blob/master/Figure3.PNG)
