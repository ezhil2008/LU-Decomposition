# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Ezhil Nilavan E
RegisterNumber: 26018188
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Ezhil Nilavan E
RegisterNumber: 26018188
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pi=lu_factor(a)
x=lu_solve((lu,pi),b)
print(x)
```

## Output:
<img width="1205" height="452" alt="Screenshot 2026-10-17 090020" src="https://github.com/user-attachments/assets/0fdcaa2e-b24a-4308-aa6b-88889181b339" />
<img width="1205" height="190" alt="Screenshot 2026-10-17 090046" src="https://github.com/user-attachments/assets/ce7cf5b7-ada9-42ab-906c-0ae25a384b3e" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

