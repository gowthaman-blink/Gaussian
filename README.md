# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: ak gowthaman
RegisterNumber: 25017622
*/
```
import numpy as np

import sys

n=int(input())

a=np.zeros((n,n+1))

x=np.zeros(n) for i in range (n):

for j in range (n+1): a[i][j]=float(input())

for i in range (n):

sys.exit('Divide by zero detected!')

if a[i][j]==0:

for j in range (i+1,n): ratio=a[j][i]/a[i][i]

for k in range (n+1):

a[j][k]=a[j][k]-ratio*a[i][k]

x[n-1]=a[n-1][n]/a[n-1][n-1]

for i in range (n-2,-1,-1):

x[i]=a[i][n]

for j in range(i+1,n):

x[i]=x[i]-a[i][j]*x[j]

for i in range(n):

x[i]=x[i]/a[i][i]

print('X%d=%0.2f'%(i,x[i]),end=' ')
## Output:
![gaussian elimination]()
![WhatsApp Image 2025-11-04 at 08 13 56_32d459ca](https://github.com/user-attachments/assets/d17194cc-b210-4e4e-b3c2-394a46f4c1c2)


## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

