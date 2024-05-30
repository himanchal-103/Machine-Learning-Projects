# LINEAR REGRESSION IMPLEMENTATION

## Aim
This project aims to implement and compare a self-built linear regression algorithm with gradient descent and the linear regression algorithm provided by Scikit-Learn. The goal is to predict whether a person has insurance based on their age.

## Dataset
The dataset contains data on whether a person of a certain age has insurance. The dataset used in this project is a self-built dummy data that has 50 records. It contains:

Feature Column: Age of a person
Target Column: Insurance(1 if the person has insurance or 0 if the person does not have insurance)

## Model
Linear Regression is the most basic algorithm in Machine Learning. It is a regression algorithm, which means that it is useful when we are required to predict continuous values, that is, the output variable ‘y’ is continuous.

Linear regression assumes a linear relation between x and y. The hypothesis function for linear regression is:

1. **For 1D data** : y = m.x + c
2. **For multi-dimensinal data** : y = (m1 * x1) + (m2 * x2) + (m3 * x3) + … + (m_n * x_n) + c

where m, m1, m2, m3 are called the parameters and c is the intercept of the line.

**m = (x*y).mean() - x.mean(). y.mean()/x^2.mean()-x.mean().x.mean()**

**c = y.mean()-m*x.mean()**

## Cost Function

A cost function is defined as a function that maps an event or values of one or more variables onto a real number intuitively representing some “cost” associated with the event. In Linear Regression the objective is to find a line of best fit for some given inputs, or X values, and any number of Y values, or outputs.

**Cost(C)= \sum_i$ $( y_i - (m.x_i + b))^2**


## Gradient Descent

Gradient descent is an optimization algorithm used to find the values of parameters (coefficients) of a function (f) that minimizes a cost function (cost). Gradient descent is best used when the parameters cannot be calculated analytically (e.g. using linear algebra) and must be searched for by an optimization algorithm.

## Learning Rate

How big the steps gradient descent takes into the direction of the local minimum are determined by the learning rate, which figures out how fast or slow we will move towards the optimal weights.

![gradient-descent-learning-rate-7052](https://github.com/himanchal-103/Machine-Learning-Projects/assets/133697230/5c3bd04c-04c0-489b-8d63-da3e37575e0a)


