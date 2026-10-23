# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Shaik Sophie Fatima
RegisterNumber: 212224043002
import numpy as np
import matplotlib.pyplot as plt

# Input data

x = np.array([1, 2, 3, 4, 5])
y = np.array([2, 4, 5, 4, 5])

# Calculate the mean

x_mean = np.mean(x)
y_mean = np.mean(y)

# Calculate slope (m)

m = np.sum((x - x_mean) * (y - y_mean)) / np.sum((x - x_mean) ** 2)

# Calculate intercept (b)

b = y_mean - m * x_mean

# Predict y values

y_pred = m * x + b

# Display results

print("Slope (m):", round(m, 2))
print("Intercept (b):", round(b, 2))
print("Best Fit Line: y =", round(m, 2), "x +", round(b, 2))

# Plot the data and regression line

plt.scatter(x, y, color='blue', label='Actual Data')
plt.plot(x, y_pred, color='red', label='Best Fit Line')
plt.xlabel("X Values")
plt.ylabel("Y Values")
plt.title("Univariate Linear Regression")
plt.legend()
plt.show()

*/
```

## Output:
<img width="805" height="672" alt="image" src="https://github.com/user-attachments/assets/d2ab615c-34e9-4796-a86a-7f958bff5bbc" />



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
