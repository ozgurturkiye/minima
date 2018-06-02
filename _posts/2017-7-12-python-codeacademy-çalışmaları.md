---
layout: post
title: codeacademy python çalışmaları
---

### Liste ve sözlük kulllanımına örnek:

```python

shopping_list = ["banana", "orange", "apple"]

stock = {
    "banana": 6,
    "apple": 0,
    "orange": 32,
    "pear": 15
}

prices = {
    "banana": 4,
    "apple": 2,
    "orange": 1.5,
    "pear": 3
}

# Write your code below!
def compute_bill(food):
    total = 0
    for fd in food:
        if stock[fd] > 0:
            total += prices[fd]
            stock[fd] -= 1
    return total

result = compute_bill(["banana", "orange"])
print(result)

```

### Sınıf not hesaplama programına örnek:

```python

lloyd = {
    "name": "Lloyd",
    "homework": [90.0, 97.0, 75.0, 92.0],
    "quizzes": [88.0, 40.0, 94.0],
    "tests": [75.0, 90.0]
}
alice = {
    "name": "Alice",
    "homework": [100.0, 92.0, 98.0, 100.0],
    "quizzes": [82.0, 83.0, 91.0],
    "tests": [89.0, 97.0]
}
tyler = {
    "name": "Tyler",
    "homework": [0.0, 87.0, 75.0, 22.0],
    "quizzes": [0.0, 75.0, 78.0],
    "tests": [100.0, 100.0]
}

# Add your function below!
def average(numbers):
    total = sum(numbers)
    return float(total) / len(numbers)


def get_average(student):
    homework = average(student['homework'])
    quizzes = average(student['quizzes'])
    tests = average(student['tests'])
    return 0.1 * homework + 0.3 * quizzes + 0.6 * tests


def get_letter_grade(score):
    if score >= 90:
        return "A"
    elif score >= 80:
        return "B"
    elif score >= 70:
        return "C"
    elif score >= 60:
        return "D"
    else:
        return "F"


def get_class_average(students):
    results = []
    for student in students:
        results.append(get_average(student))

    return average(results)


students = [lloyd, alice, tyler]

get_letter_grade(get_average(lloyd))
print(get_class_average(students))
print(get_letter_grade(get_class_average(students)))

```

#### while ile y/n sorusu

```python

choice = raw_input('Enjoying the course? (y/n)')

while choice != "y" and choice != "n":  # Fill in the condition (before the colon)
    choice = raw_input("Sorry, I didn't catch that. Enter again: ")

```
