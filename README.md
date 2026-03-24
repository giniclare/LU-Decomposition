# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module to use the built in function for calculation
2. Prepare the list from each equations anad assign in np .array()
3. using the appropriate command we can find the solution
4. End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Gini Clare G
RegisterNumber:212225240041 
'''
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
P, L, U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:Gini Clare G 
RegisterNumber:212225240041 
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve

A=np.array([[3,2,7],[2,3,1],[3,4,1]])
b=np.array([4,5,7])
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
<img width="1427" height="637" alt="Screenshot 2026-03-24 130410" src="https://github.com/user-attachments/assets/3a75f7ba-96b8-4fc4-a433-1d6d0bc59e06" />
<img width="1361" height="803" alt="Screenshot 2026-03-24 130437" src="https://github.com/user-attachments/assets/0a0d0541-6f7c-4e49-836c-43bd27fbabf7" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

