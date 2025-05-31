# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Input the matrix A from the user.
2. Perform LU decomposition on A to obtain P, L, U such that PA = LU.
3. Extract the lower triangular matrix L and upper triangular matrix U.
4. Print the matrices L and U.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Rohit GP
RegisterNumber: 2122242220082
*/

import numpy as np
from scipy.linalg import lu,solve_triangular

a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Rohit GP
RegisterNumber: 2122242220082
*/

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu,solve_triangular
a=np.array(eval(input()))
b=np.array(eval(input()))
p,l,u=lu(a)
pb=np.dot(p,b)
y=solve_triangular(l,pb,lower=True)
x=solve_triangular(u,y)
print(x) 
```

## Output:


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

