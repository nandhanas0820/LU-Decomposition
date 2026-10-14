# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
# 5a
1. import the numpy and scipy libraries
2. define the input matrix a
3. perform LU decomposition to obtain P,L and U
4. print the L and U matrices
# 5b
1. import the numpy and scipy libraries
2. get the coefficient matrix a and constant matrix b as input
3.  perform LU factorization and solve the equations to obtain X
4.  print the solution matrix X

## Program:
# (5a) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
```
# (5b) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: 
RegisterNumber: 
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:
# (5a)
<img width="1311" height="798" alt="Screenshot 2026-10-14 090559" src="https://github.com/user-attachments/assets/2c6b1d4d-fd67-4405-bfbe-68137c1b9bc0" />
# (5b)
<img width="1257" height="807" alt="Screenshot 2026-10-14 090627" src="https://github.com/user-attachments/assets/e6a02fd9-c5b5-425b-9c5f-afd4cdb3f439" />


## Result:
# (5a)
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.
# (5b)
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

