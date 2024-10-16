# Simple Linear Regression Implementations

This repository contains two implementations of **Simple Linear Regression**:

1. **Using scikit-learn**: A standard and efficient solution utilizing the popular Python library for machine learning.
2. **From Scratch**: A custom implementation to understand the underlying mechanics of linear regression using basic Python code.

## Project Overview

Simple linear regression is a statistical method used to model the relationship between a dependent variable (target) and one independent variable (feature). In this project, I aim to predict the salary (**Package**) based on a student's CGPA using a linear relationship. This project helps illustrate how linear regression works in both a library setting and from the ground up.

## Dataset

The dataset consists of two columns:
- **CGPA**: Represents the student's cumulative grade point average.
- **Package (Salary)**: Represents the salary the student is offered after graduation.

### CSV File Structure

Make sure to place the `data.csv` file in the root directory of the project. The CSV file should have the following structure:

```csv
CGPA,Package
7.5,45000
8.2,50000
7.9,47000
...
```

## Implementations

### 1. Scikit-learn Implementation

In the `sklearn_linear_regression.py` file, I implement simple linear regression using the `LinearRegression` class from the scikit-learn library. This method is efficient and simple, widely used in machine learning tasks.

#### Steps:
1. Load the dataset.
2. Split the dataset into features (CGPA) and target (Package).
3. Train the model using `model.fit()`.
4. Predict salaries using `model.predict()` for given CGPA values.

### 2. Scratch Implementation

In the `scratch_linear_regression.py` file, I implement linear regression from scratch. This implementation aims to help you understand the mathematical concept behind the algorithm without relying on external libraries.

#### Closed-form Solution

The custom implementation uses the closed-form solution to calculate the best-fitting line based on the training data. This method calculates the slope (`m`) and intercept (`b`) of the line that minimizes the error between the predicted and actual values.

#### Code Explanation

The class `SimpleLinearRegression` in `scratch_linear_regression.py` contains two main methods:
- **`__init__`**: Initializes the slope (`m`) and intercept (`b`) as `None`.
- **`fit(X_train, y_train)`**: Calculates the slope and intercept using the training data:
  - The slope (`m`) is calculated using the formula:
  m= 
 
∑(X 
i
​
 − 
X
ˉ
 )(Y 
i
​
 − 
Y
ˉ
 )/
∑(X 
i
​
 − 
X
ˉ
 ) 
2
  - 
- **`predict(X_test)`**: Uses the calculated slope and intercept to predict the salary for new CGPA values using the formula:
  \[
  Y = m \cdot X + b
  \]
  where \(Y\) is the predicted salary, \(X\) is the CGPA value, \(m\) is the slope, and \(b\) is the intercept.


## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/ashishshah1995/simple-linear-regression-implementations.git
   ```

2. Navigate to the project directory:
   ```bash
   cd simple-linear-regression-implementations
   ```

3. Run the scikit-learn implementation:
   ```bash
   python sklearn_linear_regression.py
   ```

4. Run the scratch implementation:
   ```bash
   python scratch_linear_regression.py
   ```

## Conclusion

This project demonstrates two approaches to implementing simple linear regression:
- The scikit-learn version offers a quick and reliable method using a well-optimized library.
- The scratch implementation provides insights into how linear regression works, enhancing the understanding of the underlying math and algorithm.

By comparing both approaches, I gain a deeper understanding of the mechanics behind simple linear 
