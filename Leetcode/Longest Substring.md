Problem Analysis:
================
longest substring without repeating characters
---------------
Given a string, find the length of the longest substring without repeating characters.

Programming Implementation:
==========================
```python
    def lengthLongestSubstring(s):
        leng = 0
        if s is None or len(s) == 0:
            return leng
        st= {}
        onemax = 0
        start = 0
        for i in range(len(s)):
            if s[i] in st and st[s[i]] >= start:
                start = st[s[i]] + 1
            onemax = i - start + 1
            st[s[i]] = i
            max = max(leng, onemax)
        return leng
```
Summarize:
=======
The Second string begins when the first string repeats.
