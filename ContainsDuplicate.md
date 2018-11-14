Problem Analysis:
=================
Contains Duplicate:
==========
Given an array of integers, find if the array contains any duplicates.
Your function should return true if any value appears at least twice in the array, and it should return false if every element is distinct.

Programming Implementation:
====================
Method 1
```python
 def containsDuplicate(nums):
        l=len(nums)
        for i in range(l-1):
            for j in range(i+1,l):
                if (nums[i]==nums[j]):
                    print(True)
                    break
        print(False)
 ```
Method 2
```python
 from collections import Counter
 def containsDuplicate(nums):
        c=Counter(nums)
        for i in c.values:
            if i>=2:
                print(True)
        print(False)
```
Method 3
```python
def containsDuplicate( nums):
    new=set(nums)
    if(len(new)==len(nums)):
        return True
    else:
        return False
```
Summarize:
=======
Firstly, I use a method of double loop. After referring to the answer, it is much simpler to use the Counter() and set() method.Counter is a class that inherits a dictionary. It is used to track the number of values. Pay attention to the result of key-value pairs.Set() creates an unordered set of nonrepeating elements.
