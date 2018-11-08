Problem Analysis:
=================

python
def maxProfit(prices):
    profit=0
    length=len(prices)-1
    for i in range(0,length):
        for j in range(i+1,length):
            pri=prices[j]-prices[i]
            if (profit<pri):
                profit=pri
    return profit
stockprices=[7,1,5,3,6,4]
print(maxProfit(stockprices))
```python
