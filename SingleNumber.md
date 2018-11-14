
Problem Analysis:
=================
Single Number
---------------
Given a non-empty array of integers, every element appears twice except for one. Find that single one.

Programming Implementation:
====================
Method 1
```python
from collections import Counter
def singleNumber(nums):
    c=Counter(nums)
    for key,value in c.items():
        if value==1:
            print(key)
`````
Method 2
```python
def singleNumber(nums):
    for i in nums:
        if (nums.count(i)==1):
            print(i)
 ```
Summarize:
=======
I want to firstly use the method of counter(). But I have to find how to get the value of key. The method of count() in this answer is obviously much simpler. Count() is used to count the number of a character.
