# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.
## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm
1.import libraries
2.get the matrix from the user
3.find L and U
4.print the solution 
## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: harish
RegisterNumber:23013571
import numpy as np
n=int(input())
arr=np.zeros((n,n+1))
res=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
res[n-1]=arr[n-1][n]/arr[n-1][n-1]
for i in range(n-1,-1,-1):
    res[i]=arr[i][n]
    for j in range(i+1,n):
        res[i]=res[i]-arr[i][j]*res[j]
    res[i]=res[i]/arr[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,res[i]),end=" ")
*/
```
## Output:
![image](https://github.com/Harishragaventhira/Gaussian/assets/145548269/2cc39f6f-6f4c-472e-9417-68c27bdd67e2)
## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

