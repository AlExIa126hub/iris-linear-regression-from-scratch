# Linear Regression on the Iris Dataset

Machine Learning practical assignment exploring linear regression using Fisher’s Iris dataset.

The goal of the project is to model relationships between different flower measurements by predicting one feature based on another using a simple linear regression model implemented from scratch.

Dataset source:  
https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html


---

# Project Structure

```
iris-linear-regression/
│
├── iris_linear_regression.ipynb
└── README.md
```

---

# Project Overview

Although the Iris dataset is typically used for classification problems, this project explores it from a regression perspective.

The objective is to predict one feature of the dataset using another feature through a simple linear regression model.

The project focuses on understanding the mechanics of linear regression by implementing the training process manually rather than relying on built-in machine learning functions.

The workflow includes:

1. Selecting pairs of independent and dependent variables  
2. Visualising the relationships between variables  
3. Implementing linear regression from scratch  
4. Minimising prediction error using optimisation techniques  

---

# Dataset

The Iris dataset is one of the most widely used datasets in machine learning. It contains measurements of iris flowers belonging to three species:

- Setosa  
- Versicolor  
- Virginica  

Each observation includes four features:

- sepal length  
- sepal width  
- petal length  
- petal width  

In this project, these features are used both as **independent variables (predictors)** and **dependent variables (targets)** in regression experiments.

---

# Regression Experiments

Several pairs of variables were selected in order to explore linear relationships between different flower measurements.

Examples include:

- sepal length → sepal width  
- petal length → petal width  
- petal width → sepal length  

For each pair:

1. The data is visualised using scatter plots.
2. A linear regression model is fitted.
3. The regression line is displayed on the plot.

---

# Linear Regression Implementation

The regression model is implemented manually to better understand how the algorithm works.

The model follows the standard linear regression formula:

```
y = β0 + β1x
```

Where:

- **β0** represents the intercept  
- **β1** represents the slope (coefficient)  
- **x** is the independent variable  
- **y** is the predicted value  

---

# Error Function

Model performance is evaluated using **Mean Squared Error (MSE)**.

```
MSE = (1/n) * Σ(y_true - y_pred)^2
```

The objective of the training process is to minimise this error.

---

# Optimisation Approaches

Two optimisation strategies are explored.

### Random Search

The intercept and slope are randomly initialised and repeatedly adjusted.  
For each pair of coefficients, the Mean Squared Error is calculated and the best values are kept.

Although simple, this approach demonstrates the basic concept of optimisation in machine learning.

### Improved Optimisation

A more efficient optimisation strategy is later introduced to obtain better regression coefficients and reduce the error more effectively.

---

# Visualisation

For each regression experiment, the following visualisations are produced:

- scatter plot of the original data  
- fitted regression line  
- comparison between predicted and observed values  

These visualisations help illustrate how well the linear model captures relationships between variables.

---

# Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Jupyter Notebook  

---

# Running the Project

Install dependencies:

```
pip install numpy pandas matplotlib
```

Launch Jupyter Notebook:

```
jupyter notebook
```

Open and run:

```
iris_linear_regression.ipynb
```

---

# Dataset

Iris Dataset (Scikit-learn)

https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html
