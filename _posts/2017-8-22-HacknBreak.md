---
layout: post
title: HacknBreak akşam çalışma notları!
date: 2017-08-22 Salı
---

## HacknBreak Kampı akşam çalışma notları.

1. CodeAcademy üzerinde REST nedir çalışması. [link](https://www.codecademy.com/en/courses/python-intermediate-en-6zbLp/2/2?curriculum_id=519247280cc11e2fca00330a)
2. The Anatomy of Request
  1. request line
  1. header
  1. body
3. Anatomy of a Response
  1. HTTP Response yapısı HTTP Request yapısının bir aynası gibidir.  
  1. Status code ile başlar, sunucu ve Response hakkında ek bilgiler ile devam eder. Body kısmında text mesajı ile son bulur. Örnek olarak 404 dönen sayfalarda body içinde "file not found" olur.

## XML parsing örneği
**python kodu**

```python
from xml.dom import minidom

f = open('pets.txt', 'r')
pets = minidom.parseString(f.read())
f.close()

names = pets.getElementsByTagName('name')
for name in names:
	print(name.firstChild.nodeValue)
```
**XML kodu  pets.txt**

```xml
<pets>
  <pet>
    <name>Jeffrey</name>
    <species>Giraffe</species>
  </pet>
  <pet>
    <name>Gustav</name>
    <species>Dog</species>
  </pet>
  <pet>
    <name>Gregory</name>
    <species>Duck</species>
  </pet>
</pets>
```
## JSON Parsin örneği

**python kodu**
```python
import json
from pprint import pprint

f = open('pets.txt', 'r')
pets = json.loads(f.read())
f.close()

pprint(pets)
```
**JSON Kodu pets.txt**

```json
{
  "pets": [
    {
      "name": "Jeffrey",
      "species": "Giraffe"
    },
    {
      "name": "Gustav",
      "species": "Dog"
    },
    {
      "name": "Gregory",
      "species": "Duck"
    }
  ]
}
```
