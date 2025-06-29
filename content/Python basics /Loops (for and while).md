---
title: Loops (For And While)
date: 2025-06-30
author: Your Name
cell_count: 2
score: 0
---

```python
print("Counting to 5:")
for i in range(1, 6):
    print(i)


count = 0
print("\nWhile loop example:")
while count < 3:
    print(f"Count is {count}")
    count += 1

print("\nLoop control:")
for num in range(10):
    if num == 2:
        continue  
    if num == 7:
        break     
    print(num)
```

    Counting to 5:
    1
    2
    3
    4
    5
    
    While loop example:
    Count is 0
    Count is 1
    Count is 2
    
    Loop control:
    0
    1
    3
    4
    5
    6



```python

```


---
**Score: 0**