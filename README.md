# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1: Start the Program

### Step 2: numpy for matrix creation and handling.

### Step 3: scipy.linalg.lu for LU decomposition.

### Step 4: Input the Matrix

### Step 5: Take the square matrix A as input.

### Step 6: Use eval(input()) to allow entry in Python list format (e.g., [[2,3],[4,5]]).

### Step 7: Use lu(A) from SciPy which returns:

P: Permutation matrix (accounting for row swaps),

L: Lower triangular matrix with 1s on the diagonal,

U: Upper triangular matrix.

### Step 8: Print the Lower triangular matrix (L).

### Step 9: Print the Upper triangular matrix (U).
## Program:
(i) To find the L and U matrix
```python

'''Program to find L and U matrix using LU decomposition.
Developed by: THARUN P S
RegisterNumber: 212224110055
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U) 

```
## (ii) To find the LU Decomposition of a matrix
## Algorithm

### Step 1: Start the Program

### Step 2: numpy for matrix input and handling.

### Step 3: lu_factor and lu_solve from scipy.linalg for LU decomposition and solving.

### Step 4: Input the coefficient matrix A (square matrix).

### Step 5: Input the right-hand side vector or matrix B.

### Step 6: Use lu_factor(A) to compute:

LU: combined LU decomposition matrix,

PV: pivot indices for row permutations.

### Step 7: Use lu_solve((PV, LU), B) to solve the system Ax = B.

### Step 8: Output the result vector x which solves Ax = B.
```python

'''Program to solve a matrix using LU decomposition.
Developed by: THARUN P S
RegisterNumber: 212224110055
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu,piv = lu_factor(A)
X = lu_solve((lu,piv),b)
print(X) 

```

## Output:
(i) To find the L and U matrix:
![image](https://github.com/user-attachments/assets/38d20e98-4d99-436c-bffc-cc07f227bcac)

(ii) To find the LU Decomposition of a matrix
![image](https://github.com/user-attachments/assets/01d6f8d0-f10a-430a-8fd8-34290645aa07)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

