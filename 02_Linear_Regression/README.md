# Linear Regression

- As the beginning, I have struggled a lot when studying this field so If you don't understand, don't worry about that, take a break and comeback to study later.

---

## Introduction

### What is Linear Regression?

- This is a method for you to approximate a linear relationship between 2 variables.
- For simple, Its will take your input and produce output for you. Note that the output is just a prediction that approximate the right answer, but it's not the right answer.

### When to use it?

- It is used when you want to predict **continuous dependent variable** from a number of independent variable.

### There are 2 ways I know to handle linear regression:

I will go through each of this below.

- **Normal equation:** this method directly compute the model parameters that best fits the model to the training set. Other way to explain, It compute the model parameters that minimize the cost function directly
- **Gradient descent:** this method using an iterative optimization approach to compute the model parameters over the time to minimize the cost function.

## The general form of linear regression

- check out this [video](https://www.youtube.com/watch?v=zPG4NjIkCjc&t=1s) for general idea of linear regression

**We have know that what is the linear regression model prediction. I just summarize some important thing about this:**

1. **Equation form:**

    <!-- $\hat{y} = \theta_0 + \theta_1x_1 + \theta_2x_2 + ... + \theta_nx_n$ -->
    <a href="https://www.codecogs.com/eqnedit.php?latex=\hat{y}&space;=&space;\theta_0&space;&plus;&space;\theta_1x_1&space;&plus;&space;\theta_2x_2&space;&plus;&space;...&space;&plus;&space;\theta_nx_n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\hat{y}&space;=&space;\theta_0&space;&plus;&space;\theta_1x_1&space;&plus;&space;\theta_2x_2&space;&plus;&space;...&space;&plus;&space;\theta_nx_n" title="\hat{y} = \theta_0 + \theta_1x_1 + \theta_2x_2 + ... + \theta_nx_n" /></a>

    - $\hat{y}$ is the predicted value
    - n is the number of features
    - $x_i$ is the $i^{th}$ feature value
    - $\theta_j$ is the $j^{th}$ model parameter ( including the bias term $\theta_0$ and the feature weights $\theta_1, \theta_2, ...,\theta_n$ )
2. **MSE cost function:**

    $J(\theta) = \frac1m \sum_{i=1}^m (\theta^T x^{(i)} - y^{(i)})^2$

3. **Our target is to find the model parameter (or feature weights) $\theta$ to minimize the cost function above**