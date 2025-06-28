---
title: Control Flow (If, Elif, Else)
date: 2025-06-29
author: Your Name
cell_count: 2
score: 0
---

```python

age = 18
if age >= 18:
    print("You are an adult")
else:
    print("You are a minor")


score = 85
if score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
elif score >= 70:
    grade = 'C'
else:
    grade = 'D'
print(f"Your grade is {grade}")


is_even = "Even" if (age % 2 == 0) else "Odd"
print(f"{age} is {is_even}")
```

    You are an adult
    Your grade is B
    18 is Even



```python

```


---
**Score: 0**