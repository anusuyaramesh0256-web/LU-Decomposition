# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. FINDING  THE  'L' AND'U' MATRIX:
STEP1:import the numpy module to use the built-in functions for calculation.
STEP2:Prepare the lists from each linear equations and assign in np.array().
STEP3:Using the P,L,U = lu(),we get two results (first is L and second is U)of the given matrix.
STEP4:end te program.
2. FINDING DECOMPOSITION OF THE MATRIX:
STEP1:import the numpy module to use the built-in functions for calculation.
STEP2:Prepare the lists from each linear equations and assign in np.array().
STEP3:Using the pivot=lu_factor(A) and lu_solve((lu,pivot),B),we can find results the LU Decompostion of a matrix.



## Program:
~~~
(i) To find the L and U matrix
'''Program to find L and U matrix using LU decomposition.
Developed by: ANUSUYA R
RegisterNumber: 212225220010
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
~~~

(ii) To find the LU Decomposition of a matrix
~~~
'''Program to solve a matrix using LU decomposition.
Developed by: ANUSUYA R 
RegisterNumber: 212225220010
'''

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)

~~~

## Output:
![alt text](<Screenshot 2026-03-23 195116.png>)
![alt text](<Screenshot 2026-03-23 195258.png>)
![alt text](<Screenshot 2026-03-23 195332.png>)
![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

