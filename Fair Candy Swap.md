```python
def fairCandySwap(self, A, B):
        Sa, Sb = sum(A), sum(B)
        setB = set(B)
        for x in A:
            y=int(x + (Sb - Sa) / 2)
            if y in setB:
                return [x, y]
