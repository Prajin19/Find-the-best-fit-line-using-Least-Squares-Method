# Implementation of Univariate Linear Regression
# Name : Prajin S
# Register Number : 212223230151
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

```Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Prajin S
RegisterNumber: 212223230151
```
``` Python
import numpy as np
import matplotlib.pyplot as plt
```
``` Python
a=np.array(eval(input()))
b=np.array(eval(input()))
```
![image](https://github.com/user-attachments/assets/27512d49-c179-44de-bf9b-a597a179f9ce)

``` Python
abar=np.mean(a)
bbar=np.mean(b)
print(abar,bbar)
```
![image](https://github.com/user-attachments/assets/ee23af1c-42bd-4572-8c26-b65ac3243a4c)

``` Python
num,den=0,0
for i in range(len(a)):
    num+=((a[i]-abar)*(b[i]-bbar))
    den+=(a[i]-abar)**2
m=num/den
print(m)
```
![image](https://github.com/user-attachments/assets/ba1e401b-60ab-4de8-b6fc-7783ef514dfa)

``` Python
c=bbar-m*abar
print(c)
```
![image](https://github.com/user-attachments/assets/e3fa09d8-061c-4044-8e5f-b81db2bead01)

``` Python
ycal=m*a+c
ycal
```
![image](https://github.com/user-attachments/assets/773284b0-591c-4523-a2d8-5bb4e405a101)

``` Python
plt.scatter(a,b,color='black')
plt.plot(a,ycal,color='orange')
plt.show()
```
![image](https://github.com/user-attachments/assets/671526d8-c92f-4953-ae3f-7faa84870dc8)

## Output:
![image](https://github.com/user-attachments/assets/7971d040-6612-4d59-ba2b-7296650d5a08)
![image](https://github.com/user-attachments/assets/9d65f6e6-08bc-4d53-b71d-ec1af2383cf4)



## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
