# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program and import the required libraries (NumPy and SciPy).  
2.Define the matrix using NumPy.  
3.Use lu() to perform LU decomposition and display the lower and upper triangular matrices.  
4.Use lu_factor() and lu_solve() to factorize the matrix and solve the system of equations.  
5.Display the solution and end the program. 
## Program:
(i) To find the L and U matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
'''Program to find L and U matrix using LU decomposition.
Developed by: G.Sushanth
RegisterNumber: 212225230088
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
import  os
os.environ["OPENBLAS_NUM_THREADS"]="1"
'''Program to solve a matrix using LU decomposition.
Developed by:G.Sushanth
RegisterNumber: 212225230088
'''
# To print X matrix (solution to the equations)

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu , piv),b)
print(X)

```

## Output:
<img width="1211" height="447" alt="{BD256B39-D5D3-4E6E-8F58-F56BAD52A0D9}" src="https://github.com/user-attachments/assets/ab8443e9-31d5-4bf4-b48b-6b0f3c446d08" />

<img width="1163" height="200" alt="{78409CCF-E3B5-4366-BF9F-A6C426583172}" src="https://github.com/user-attachments/assets/5308bc02-c07a-45cd-947d-34bbea84ec6a" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

