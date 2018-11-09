Problem Analysis:
================


```python
def Rotate(nums,k):
    l=len(nums)
    k=k%l
    nums[:]=nums[l-k:]+nums[:l-k]
    return nums
```
