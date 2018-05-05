---
title: "Intro to Machine Learning: Linear Regression and Ridge Regression"
date: 2018-02-02
tags: [machine learning, Linear Regression, Ridge Regression, MNIST digit prediction]
excerpt: "Machine Learning, Linear Regression, Ridge Regression, MNIST digit prediction" 
---

# Intro to Machine Learning: Linear Regression and Ridge Regression

1. Linear Regression
    Dataset: linRegData.npy
    The data is a matrix (100, 2). Column 1 is x and Column 2 is y.
    Data is be read using numpy.load(’linRegData.npy’). Given a function $$y = f(x)$$, using linear
    regression a program to find the line which best fits the data. 

    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/Intro-to-ML/Linear-Reg.png" alt="fitting linear curve"/>

2. Ridge Regression
    Dataset: linRegData.npy
    The data is a matrix (100, 2). Column 1 is $$x$$ and Column 2 is $$y$$.
    Data can be read using $$numpy.load(’linRegData.npy’)$$. For this exercise, fit a polynomial of degree
    15 to the data using ridge regression. I.e. $$x$$ is converted to $$[1, x, x^2, x^3, . . . , x^15]^T$$. Using 5-fold cross
    validation, estimating the best $$λ$$ from the set, $$λs = [0.01; 0.05; 0.1; 0.5; 1.0; 5; 10];$$
    
    <img src="{{ site.url }}{{ site.baseurl }}/assets/images/Intro-to-ML/Ridge-Regression.png" alt="fitting a non-linear curve"/>


