Problem Analysis:
=========
PlusOne
-------
Given a non-empty array of digits representing a non-negative integer, plus one to the integer.
The digits are stored such that the most significant digit is at the head of the list, and each element in the array contain a single digit.

```python
def plusOne(digits):
    l=len(digits)
    a=0
    for i in range(l):
        nums=digits[i]
        a+=nums*(10**(l-i-1))
    intdigits=a+1
    strdigits=str(intdigits)
    res=[]
    for j in range(len(strdigits)):
        res.append(int(strdigits[j]))
    print(res)
```
Programming Implementation:
===========
Flexible use of conversions between characters and integers.
