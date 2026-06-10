# LU Decomposition 

## AIM:

To write a program to find the LU Decomposition of a matrix.

## Equipments Required:

1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

1. Read the order n and the elements of the square matrix A.
  
2. Initialize L as an identity matrix and U as a zero matrix.

3. Compute the elements of L and U using LU Decomposition formulas.

4. Display the matrices L and U and stop.

## Program:

(i) To find the L and U matrix
```
Program to find the L and U matrix.
Developed by: Tejasvi S
RegisterNumber: 212225040465
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
Program to find the LU Decomposition of a matrix.
Developed by: Sivasakthi S
RegisterNumber: 212225040418
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot= lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:

(i)

<img width="1231" height="474" alt="Screenshot 2026-05-14 141450" src="https://github.com/user-attachments/assets/740b27be-cec8-449c-be3b-a263cd1382b2" />

(ii)

<img width="1220" height="207" alt="Screenshot 2026-05-14 141513" src="https://github.com/user-attachments/assets/4276128c-c273-4837-8e00-a158f2e10f6e" />

## Result:

Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

