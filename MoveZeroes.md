Problem Analysis:
========
Move Zeroes
--------
Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.
Programming Implementation:
===========
```python
def moveZeroes(nums):
    l1=len(nums)
    while 0 in nums:
        nums.remove(0)
    l2=len(nums)
    zeron=l1-l2
    for i in range(zeron):
        nums.append(0)
    print(nums)
```
others
```python
def moveZeroes(nums):
        for num in nums:
            if num==0:
                nums.remove(0)
                nums.append(0)
        return nums
```
Summarize:
=======
I should be flexiblely use of remove and append.
