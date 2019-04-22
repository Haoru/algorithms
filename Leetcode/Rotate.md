Problem Analysis:
================
Ratate The Arrary
--------------

Given an array, rotate the array to the right by k steps, where k is non-negative.

Programming Implementation:
==========================
```python
def Rotate(nums,k):
    l=len(nums)
    k=k%l
    nums[:]=nums[l-k:]+nums[:l-k]
    return nums
```

Summarize:
=======

Slices can extract a portion of the list.Be sure to pay attention to the index.
