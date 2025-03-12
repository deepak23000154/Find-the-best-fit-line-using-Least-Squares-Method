# Ex-1:Implementation of Univariate Linear Regression

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
Program to implement univariate Linear Regression to fit a straight line using least squares.<br>
Developed by: DEEPAK.R<br>
Register Number: 212223040031<br>

```
import numpy as np
import matplotlib.pyplot as plt
X=np.array(eval(input()))
Y=np.array(eval(input()))
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='red')
plt.plot(X,Y_pred,color='grey') 
plt.show() 
```

## Output:
### X and Y Values
![1)](https://github.com/user-attachments/assets/b4e27c65-cb28-467a-9a36-56f6117c21f2)
### X_mean and Y_mean
![2)](https://github.com/user-attachments/assets/cb7c3cf8-603f-40aa-a1b3-f85a16be87f5)
### Slope and Intercept
![3)](https://github.com/user-attachments/assets/01a3b20e-3d19-4ad4-a1d5-81455fdde280)
### Predicted Y Values
![4)](https://github.com/user-attachments/assets/2d784a41-3a3a-4465-8e2f-a907a9d35f4f)
### Graph
![5)](https://github.com/user-attachments/assets/c1ab16be-d1da-47c3-9802-3a4581e33f35)






## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
