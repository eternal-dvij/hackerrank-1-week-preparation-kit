# hackerrank-1-week-preparation-kit

# problem 1
*Given five positive integers, find the minimum and maximum values that can be calculated by summing exactly four of the five integers. Then print the respective minimum and maximum values as a single line of two space-separated long integers.*

Example arr = [1,3,5,7,9]

The minimum sum is 16 and the maximum sum is 24. 

The function prints

16 24


```python
#!/bin/python3

import math
import os
import random
import re
import sys

#
# Complete the 'miniMaxSum' function below.
#
# The function accepts INTEGER_ARRAY arr as parameter.
#

def miniMaxSum(arr):
    minval = min(sorted(arr))
    maxval = max(sorted(arr))
    minsum = sum(arr)-maxval
    maxsum = sum(arr)-minval
    print(str(minsum) + " " + str(maxsum))

if __name__ == '__main__':

    arr = list(map(int, input().rstrip().split()))

    miniMaxSum(arr)
```

