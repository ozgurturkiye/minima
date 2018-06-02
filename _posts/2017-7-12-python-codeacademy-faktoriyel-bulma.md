---
layout: post
title: faktoriyel bulma
---

```python

def factorial(x):
    if x < 2:
        return 1
    else:
        return x * factorial(x - 1)

print(factorial(int(input("enter number: ")))))

```
