Problem Analysis
=========
NumIsland
-----
Given a 2d grid map of '1's (land) and '0's (water), count the number of islands. An island is surrounded by water and is formed by connecting adjacent lands horizontally or vertically. You may assume all four edges of the grid are all surrounded by water.
Programming
=====
```python
import numpy as np
def numIsland(array):
    h=array.shape[0]
    l=array.shape[1]
    new_array=np.pad(array,1,'constant')
    num=0
    for i in range(1, l+1):
        for j in range(1,h):
            if new_array[i][j]==1:
                num+=1
                deep_search(i,j,new_array)
    return num
def deep_search(i,j,grid):
    if grid[i][j]==0:
        return
    grid[i][j]=0
    deep_search(i,j+1,grid)
    deep_search(i,j-1,grid)
    deep_search(i-1,j,grid)
    deep_search(i+1,j,grid)
```
test
```python
array=np.random.randint(2,size=(4,5))
print(array)
print(numIsland(array))
```
summarize
======
Queue is a first in first out stracture. The closer you get to the root, the earlier you go through it. Note padding the boundary with zero. There is a method of np.pad(). 
