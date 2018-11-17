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
