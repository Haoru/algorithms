Problem Analysis:
======
Matrix Rotate
-------

You are given an n x n 2D matrix representing an image.Rotate the image by 90 degrees (clockwise).

Programming Implementation:
================
```python
import numpy as np
def rotate(matrix):
    artmatrix=np.array(matrix)
    art1=artmatrix.T
    s=art1.shape
    print(s)
    unit=np.eye(3)
    tunit=np.dot(unit,unit)
    t2unit=np.dot(tunit,unit)
    newmatrix=np.dot(art1,tunit)
    print(newmatrix)
```
```python
import numpy as np
def rotate(matrix):
        m = len(matrix)
        n = len(matrix[0])
        matrix = zip(*matrix)
        matrix = map(list, matrix)
        for i in range(m):
            for j in range(int(n / 2)):  
                matrix[i][j], matrix[i][n - j - 1] = matrix[i][n - j - 1], matrix[i][j]
        return matrix
```
Summarize:
==========
You take the dot of the identity matrix, and you get the flip of the matrix.
