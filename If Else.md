---
share: true
---


https://www.hackerrank.com/challenges/py-if-else/problem?isFullScreen=true

Basic Solution

```python
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input().strip())
    if n % 2 != 0 :
        print("Weird")
    elif (n % 2 == 0) and (n > 2 and n < 5):
        print("Not Weird")
    elif (n % 2 == 0) and (n > 6 and n < 20):
        print("Weird")
    elif(n % 2 == 0) and (n > 20):
        print("Not Weird")
    else:
        print("Error")
```

Short Solution

```python
if n%2 != 0 or (n%2 ==0 and 6<n<=20):
    print("Weird")
elif n%2==0 and (n>20 or 2<n<5):
    print("Not Weird")
```

Shortest Solution

```python
n = int(input().strip())
if(n%2==1 or (n%2==0 and n in range(7,21))):
    print('Weird')
else:
    print('Not Weird')
```