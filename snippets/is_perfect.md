---
title: is_perfect
tags: math,intermediate
---

Checks if the provided integer is a perfect number.

- A perfect number is a number whose divisors sum to a number.
- E.g it's True for 6 (divisors 1,2,3, 1+2+3=6)
- 

```py
def is_perfect(n):
  return n==sum(i if n%i==0 else 0 for i in range(1,n//2+1))
```

```py
is_perfect(6) # True
is_perfect(13) # False
```
