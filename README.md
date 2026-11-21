# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

Algorithm:
Step 1: Start the program.

Step 2: Import the NumPy library and the required functions from the SciPy library.

Step 3: Get the elements of the matrix and store them in a variable.

Step 4: Using the lu() function, we can find the L and U matrices of the given matrix.

Step 5: Using the lu_factor() and lu_solve() functions, we can find the solution of the given system of linear equations.

Step 6: Display the L matrix, U matrix and solution matrix.

Step 7: Stop the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Abinaya P
RegisterNumber: 212225230003
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:Abinaya P 
RegisterNumber: 212225230003
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)

```

## Output:
<img width="1756" height="868" alt="Screenshot 2026-11-21 104728" src="https://github.com/user-attachments/assets/1b81f281-8ee4-46fb-bb2a-a205c917c7ba" />
<img width="1358" height="822" alt="Screenshot 2026-11-21 104738" src="https://github.com/user-attachments/assets/d76fc457-c081-496c-a890-d5a70d3ece56" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

