Problem Analysis:
=================
Find The Maximum Profit
 -------------
 Say you have an array for which the ith element is the price of a given stock on day i.
Design an algorithm to find the maximum profit. You may complete as many transactions as you like
Programming Implementation:
==========================
```python
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
