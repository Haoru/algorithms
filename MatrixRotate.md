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
Summarize:
==========
