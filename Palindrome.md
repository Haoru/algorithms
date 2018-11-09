Problem Analysis:
================
Palindrome Number
-----------------
Determine whether an integer is a palindrome. An integer is a palindrome when it reads the same backward as forward.

Programming Implementation:
==========================

```python
def isPalindrome(self, x):
n=int(input(""))
n=str(n)
m=n[::-1]
if(n==m):
    print("yes")
else:
    print("no")
```

Summarize:
=======
Pay attention to the use of slicing in python.
