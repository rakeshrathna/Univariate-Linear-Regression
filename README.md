# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
Developed by:RAKESH RATHNA M 
Register.no:212224040265
import numpy as np
from matplotlib import pyplot
X=np.array(eval(input()))
Y=np.array(eval(input()))
xmean=np.mean(X)
ymean=np.mean(Y)
num,dem=0,0
for i inrange(0,len(X)):
  num += (X[i]-xmean)*(Y[i]-ymean)
  dem += (X[i]-xmean)**2
slope=num/dem
c=ymean-slope*xmean
y_pred=slope*X+c
pyplot.scatter(X,Y,colour="blue")
pyplot.plot(X,y_pred,color="pink")
pyplot.show






```
## Output
![Screenshot 2025-05-22 140733](https://github.com/user-attachments/assets/992d0a22-d1f8-44e3-abd8-34cb0e5e42fd)

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
