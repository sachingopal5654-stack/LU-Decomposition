# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
5(a)
1. Import numpy for multi-dimensional array operations
2. Bring lu from scipy.linalg to handle the actual matrix decomposition
3. Call the lu(A) function. This splits the target matrix into three seperate output matrices P,L and U
4. End the program
5(b)
1. Import numpy for multi-dimensional array operation
2. Bring lu from scipy.linalg to handle the actual matrix decompostion
3. Pass the factorized compomemts(lu,p) along with the right-hand side matrix b into the lu_solve() function to compute the solution matrix
## Program:
(i) 5(a)To find the L and U matrix
Program to find L and U matrix using LU decomposition.
Developed by: Sachin G
RegisterNumber: 26011448
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

(ii) 5(b)To find the LU Decomposition of a matrix

Program to find the LU Decomposition of a matrix.
Developed by: Sachin G
RegisterNumber: 26011448
To print X matrix using LU decomposition
import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)

## Output:
5(a)
<img width="1177" height="1013" alt="Screenshot 2026-10-23 084230" src="https://github.com/user-attachments/assets/09e63b24-2a3a-407c-b6f5-ed2ddc67f559" />

5(b)
<img width="1172" height="757" alt="Screenshot 2026-10-23 084328" src="https://github.com/user-attachments/assets/45531bfa-59bf-427c-8c19-117b50fe9e9b" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

