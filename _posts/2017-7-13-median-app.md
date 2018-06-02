---
layout: post
title: median (ortalama bulma) app
---

Codeacademy median app example

```python

def median(orj_list):
  average = 0
  new_list = sorted(orj_list)
  list_len = len(new_list)
  print(new_list)
  print(list_len)
  if list_len % 2 == 0:
    average = (new_list[int((list_len / 2))] + new_list[int(list_len / 2 - 1)]) / 2.0
    return average
  else:
    average = new_list[int((list_len - 1) / 2)]
    return average

print(median([4, 5, 5, 4]))
```
