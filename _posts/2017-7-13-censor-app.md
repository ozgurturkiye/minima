---
layout: post
title: Sansür uygulaması-censor app
---

Codeacademy censor app example

```python

def censor(text, word):
    text_list = text.split()
    print(text_list)
    for i in range(len(text_list)):
        if text_list[i] == word:
            text_list[i] = "*" * len(word)

    text_censored = " ".join(text_list)
    return text_censored

print(censor("this hack is wack hack", "hack") )

```
