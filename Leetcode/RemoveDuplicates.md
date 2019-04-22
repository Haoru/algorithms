Problem Analysis:
=================
Remove the duplicates
----------------------
Given a sorted array nums, remove the duplicates in-place such that each element appear only once and return the new length.
Do not allocate extra space for another array, you must do this by modifying the input array in-place with O(1) extra memory.

Programming Implementation:
==========================
```python
 def removeDuplicates(nums):
        i=1
        while i <len(nums):
            if (nums[i-1]==nums[i]):
                nums.remove(nums[i])
            else :
                i+=1
        return len(nums)
number=removeDuplicates([0,0,1,2,2,3,3,3])
print(number)
```
Summarize:
=======
It's a simple array promble.I've got a loop and a judgment to check the duplicates.Pay attention to the boundary of i.  
