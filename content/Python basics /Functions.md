---
title: Functions
date: 2025-06-30
author: Your Name
cell_count: 2
score: 0
---

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))


def power(base, exponent=2):
    return base ** exponent

print(power(3))     
print(power(3, 3))   


def sum_all(*numbers):
    total = 0
    for num in numbers:
        total += num
    return total

print(sum_all(1, 2, 3, 4))  
```

    Hello, Alice!
    9
    27
    10



```python

```


---
**Score: 0**