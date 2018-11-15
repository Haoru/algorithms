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
