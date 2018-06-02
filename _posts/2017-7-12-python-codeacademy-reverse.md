---
layout: post
title: Reverse kullanmadan karakter dizilerini ters çevirme
---

```python

def reverse(text):
  text_reverse = ""
  for i in range(len(text)):
    text_reverse += text[((len(text) - 1) - i)]
  print(text_reverse)

reverse("ozgur")

```
