### Source:
[LT](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)

##### Code1(own):

```
prices = [6,1,5,3,6,4]
prices = [7,6,2,3,1]
getValue = 0
getValue1 = 0

for i in range (0,len(prices)):
    for j in range (i+1,len(prices)):
        if prices[i] < prices[j]:
            getValue = prices[j] - prices[i]
            print("minus value", getValue)
            if getValue1 < getValue:
                getValue1 = getValue
                print("minus high check", getValue1)
print (getValue1)
```

* In above code i get time complexity error

##### Code 2()