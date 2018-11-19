Problem Analysis:
=========
Reverse String
-------
Write a function that takes a string as input and returns the string reversed.
Programming Implementation:
==================
```python
def reverseString(s):
    lstr=len(s)
    new=s[::-1]
    print(new)
```
Summarize:
========
This problem refers to the slice of string. The format is \[start:end:step].Extract from start to end - 1, extract one for each step character.The position/offset of the first character on the left is 0, and the position/offset of the last character on the right is -1.
