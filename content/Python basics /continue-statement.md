---
title: Continue-Statement
date: 2025-06-30
author: Your Name
cell_count: 12
score: 10
---

```python
# Syntax of Continue Statement in Python
```


```python
for letter in 'Technology':
    if letter == 'n':
        print('Skipping the loop at', letter)
        continue
```

    Skipping the loop at n



```python
   print(letter)
```

    y



```python
for letter in 'Technology':
    if letter == 'n':
        print('Skipping the loop at', letter)
        continue
    print(letter)

```

    T
    e
    c
    h
    Skipping the loop at n
    o
    l
    o
    g
    y



```python
for x in range(1, 6):
    if x == 3:
        print('Continue without 3')
        continue # It will skip the rest iteration and go back in the for loop with the next iteration.
    print(x)
```

    1
    2
    Continue without 3
    4
    5



```python
# Displaying numbers using continue statement.
```


```python
# while loop.
```


```python
x = 1 # Initialization.
while x <= 6:
    if x == 3:
        x = x + 1
        continue
    print(x)
    x = x + 1
```

    1
    2
    4
    5
    6



```python
# Outer loop.
```


```python
for x in range(1, 4):
   # Inner loop.
     for y in range(1, 4):
       if x == 2 and y == 3:
           continue # continue statement inside the inner for loop.
       print(x,y)
```

    1 1
    1 2
    1 3
    2 1
    2 2
    3 1
    3 2
    3 3



```python
for x in range(1, 7):
    if x < 2:
        continue
    print(x)
    if x < 4:
        continue
    print(10 * x)
```

    2
    3
    4
    40
    5
    50
    6
    60



```python

```


---
**Score: 10**