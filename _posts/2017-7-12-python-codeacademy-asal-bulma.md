---
layout: post
title: Asal sayı bulma
---

Asal sayı bulma

```python

def is_prime(x):
  if x > 1:
    for i in range(2, x):
      if x % i == 0:
        return False
    else:
      return True
  else:
    return False


print(is_prime(int(input("enter number: "))))

```
