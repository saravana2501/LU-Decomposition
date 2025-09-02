# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
step 1:
Input matrix A (coefficients) and vector b (constants).

step 2:
Perform LU decomposition of matrix A to get combined LU matrix and pivot array.

step 3:
Use the LU factors to solve the linear system AX = b.

step 4:
Compute the solution vector X.

step 5:
Output the result X.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SARAVANA KUMAR S 
RegisterNumber: 212224220090
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
## Output:

<img width="789" height="576" alt="Screenshot 2025-09-02 141000" src="https://github.com/user-attachments/assets/f6f4a7a5-016d-498f-8122-52b9a8b095ec" />

(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: SARAVANA KUMAR S
RegisterNumber: 212224220090
'''

import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)

```

## Output:
![lu decomposition]()

<img width="684" height="463" alt="Screenshot 2025-09-02 141014" src="https://github.com/user-attachments/assets/8b4e3a9d-9c70-4ac8-8e3b-7e10a1220b50" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

