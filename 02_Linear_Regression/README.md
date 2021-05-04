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
    ![1](https://bit.ly/3egiSIA)

    - ![2](https://bit.ly/3ddLuPB) is the predicted value
    - n is the number of features
    - ![3](https://bit.ly/N4rBh6) is the ![4](https://bit.ly/3nSdHSk) feature value
    - ![5](https://bit.ly/3aZMoQM) is the ![6](https://bit.ly/3th9f0z) model parameter ( including the bias term ![7](https://bit.ly/3vFSsWi) and the feature weights ![8](https://bit.ly/3einbDg) )
2. **MSE cost function:**

    ![9](https://bit.ly/3xKQV39)

3. **Our target is to find the model parameter (or feature weights) ![10](https://bit.ly/2KkR7PC) to minimize the cost function above**
