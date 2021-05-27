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
- **[Gradient descent](https://www.youtube.com/watch?v=IHZwWFHWa-w):** this method using an iterative optimization approach to compute the model parameters over the time to minimize the cost function.

## The general form of linear regression

- check out this [video](https://www.youtube.com/watch?v=zPG4NjIkCjc&t=1s) for general idea of linear regression

**We have know that what is the linear regression model prediction. I just summarize some important thing about this:**

1. **Equation form:**

    <!-- $\hat{y} = \theta_0 + \theta_1x_1 + \theta_2x_2 + ... + \theta_nx_n$ -->
    <a href="https://www.codecogs.com/eqnedit.php?latex=\hat{y}&space;=&space;\theta_0&space;&plus;&space;\theta_1x_1&space;&plus;&space;\theta_2x_2&space;&plus;&space;...&space;&plus;&space;\theta_nx_n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\hat{y}&space;=&space;\theta_0&space;&plus;&space;\theta_1x_1&space;&plus;&space;\theta_2x_2&space;&plus;&space;...&space;&plus;&space;\theta_nx_n" title="\hat{y} = \theta_0 + \theta_1x_1 + \theta_2x_2 + ... + \theta_nx_n" /></a>

    - <a href="https://www.codecogs.com/eqnedit.php?latex=\hat{y}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\hat{y}" title="\hat{y}" /></a> is the predicted value
    - n is the number of features
    - <a href="https://www.codecogs.com/eqnedit.php?latex=x_i" target="_blank"><img src="https://latex.codecogs.com/gif.latex?x_i" title="x_i" /></a> is the <a href="https://www.codecogs.com/eqnedit.php?latex=i^{th}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?i^{th}" title="i^{th}" /></a> feature value
    - <a href="https://www.codecogs.com/eqnedit.php?latex=\theta_j" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\theta_j" title="\theta_j" /></a> is the <a href="https://www.codecogs.com/eqnedit.php?latex=j^{th}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?j^{th}" title="j^{th}" /></a> model parameter ( including the bias term $\theta_0$ and the feature weights <a href="https://www.codecogs.com/eqnedit.php?latex=\theta_1,&space;\theta_2,&space;...,\theta_n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\theta_1,&space;\theta_2,&space;...,\theta_n" title="\theta_1, \theta_2, ...,\theta_n" /></a> )
2. **MSE cost function:**

    <img src="https://render.githubusercontent.com/render/math?math=J(\theta) = \frac1m \sum_{i=1}^m (\theta^T x^{(i)} - y^{(i)})^2">

3. **Our target is to find the model parameter (or feature weights) <img src="https://render.githubusercontent.com/render/math?math=\theta">  to minimize the cost function above**


<!-- equation do not showing in github
https://www.codecogs.com/latex/eqneditor.php
https://gist.github.com/a-rodin/fef3f543412d6e1ec5b6cf55bf197d7b
 -->
