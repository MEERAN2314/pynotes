---
title: Variables
date: 2025-06-30
author: Your Name
cell_count: 26
score: 25
---

```python
num = 20
```


```python
print(id(num))
```

    9754472



```python
x = 20 
y = 50
z = 100
```


```python
print(x);print(y);print(z)
```

    20
    50
    100



```python
phy = 89
chem = 86
maths = 90

```


```python

marks_obtained = phy + chem + maths
```


```python
mark = (marks_obtained * 100) / 300
```


```python
print(mark)
```

    88.33333333333333



```python
x = 80 
y = 99.99
```


```python
name = 'Radhika'
```


```python
print(x); print(y); print(name);
```

    80
    99.99
    Radhika



```python
radius = 5
pi = 3.14
```


```python
perimeter = 2 * pi * radius
area = 3.14 * radius * radius
```


```python
print("Perimeter of the circle = ", perimeter)
print("Area of the circle = ", area)
```

    Perimeter of the circle =  31.400000000000002
    Area of the circle =  78.5



```python
#  Multiple Assignment
```


```python
x = y = z = 20
```


```python
print(id(x));print(id(y));print(id(z))
```

    9754472
    9754472
    9754472



```python
x = 20
y = x
z = y
```


```python
print(id(x));print(id(y));print(id(z))
```

    9754472
    9754472
    9754472



```python
 # Assigning multiple values to multiple variables:
```


```python
x, y, z = 20, 25.50, 'text'
```


```python
print(id(x));print(id(y));print(id(z))
```

    9754472
    127922448132752
    9809720



```python
fruit1, fruit2, fruit3 = "Banana", "Orange", "Mango"
```


```python
print(id(fruit1));print(id(fruit2));print(fruit3)
```

    127922219592720
    127922515726464
    Mango



```python
print(type(fruit1))
```

    <class 'str'>



```python

```


---
**Score: 25**