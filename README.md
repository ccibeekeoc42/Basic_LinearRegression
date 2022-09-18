# Basic Linear Regression Algorithm
This repo explores the basics of Linear Regression algorithm from scratch. Enjoy!

### Software, Tools, and prerequisits
1. Access to Google Colab or some Jupyter Notebook.
2. Basic python programing.
3. Basic arithmetic & calculus knowledge

### Intro: What is Linear Regression?
This deals with understanding the pattern/ slope of a given dataset given the assumption that the dataset has a linear pattern. Basically predicting the value of a variable based off the value of another variable.

Given a formulars, 
1. Equation of a line:
$$\hat{y} = wx + b$$
2. Mean Squared Error $(MSE)$, also happens to be the cost function:
$$MSE = \frac{1}{N} \Sigma_{i=1}^n({y}-\hat{y})^2$$ 
$$J(w,b) = \frac{1}{N} \Sigma_{i=1}^n({y}- (w_{i}x + b))^2$$
3. and the derivitive of the cost function:     
$J^{'}(w,b) = 
\begin{bmatrix} 
\frac{dJ}{dw} \\
\\
\frac{dJ}{db}
\end{bmatrix}
=
\begin{bmatrix} 
\frac{1}{N} \Sigma-2x_{i}({y}- (w_{i}x + b))^2 \\
\\
\frac{1}{N} \Sigma-2({y}- (w_{i}x + b))^2
\end{bmatrix}$

The derivitive (negative graidient) of the cost functions tells us which direction to go to minimize the loss/ cost function which happens to be the $MSE$ in this example.
