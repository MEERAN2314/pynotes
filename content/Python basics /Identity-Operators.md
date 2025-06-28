---
title: Identity-Operators
date: 2025-06-29
author: Your Name
cell_count: 41
score: 40
---

```python
#  Identity Is operator (is)
```


```python
x = 20
y = 20
```


```python
result = x is y
```


```python
print(result)
```

    True



```python
str1 = "Python"
str2 = "Python"
```


```python
result = str1 is str2
```


```python
print(result)
```

    True



```python
name1 = "John"
name2 = "Jack"
```


```python
result = name1 is name2
```


```python
print(result)
```

    False



```python
a = True
b = 1
```


```python
result = a is b
```


```python
print(result)
```

    False



```python
p = "20"
q = 20
```


```python
result = p is q
```


```python
print(result)
```

    False



```python
list1 = [10, 20.5, 30, 'text']
list2 = [10, 20.5, 30, 'text']
```


```python
result = list1 is list2
```


```python
print(result)
```

    False



```python

```


```python
dict1 = {
    'name': 'Jack',
    'age': 22,
}
dict2 = {
    'name': 'Jack',
    'age': 22,
}
```


```python
result = dict1 is dict2
```


```python
print(result)
```

    False



```python
tuple1 = (1, 2.5, 3, 'Technology')
tuple2 = (1, 2.5, 3, 'Technology')
```


```python
result = tuple1 is tuple2
```


```python
print(result)
```

    False



```python
# Identity Is not operator (is not)
```


```python
num1 = 30
num2 = 40
```


```python
print(num1 is not num2)
```

    True



```python
num2 = 30
```


```python
print(num1 is not num2)
```

    False



```python
str1 = 'Python'
str2 = 'Program'
```


```python
print(str1 is not str2)
```

    True



```python
list1 = [2, 4, 6, 8, 10]
list2 = [12, 14, 16]
```


```python
print(list1 is not list2)
```

    True



```python
num1 = 20
num2 = 20
```


```python
print("num1 = ", num1, " ", "id(num1): ", id(num1))
```

    num1 =  20   id(num1):  9754472



```python
print("num2 = ", num2, " ", "id(num2): ", id(num2))
```

    num2 =  20   id(num2):  9754472



```python
if(num1 is num2):
    print('num1 and num2 have the same identity')
else:
    print('num1 and num2 do not have the same identity')

if(id(num1) == id(num2)):
    print('num1 and num2 have the same identity')
else:
    print('num1 and num2 do not have the same identity')
```

    num1 and num2 have the same identity
    num1 and num2 have the same identity



```python
num2 = 40
print("num1 = ", num1, " ", "id(num1): ", id(num1))
print("num2 = ", num2, " ", "id(num2): ", id(num2))

if(num1 is not num2):
    print('num1 and num2 do not have the same identity')
else:
    print('num1 and num2 have the same identity')
```

    num1 =  20   id(num1):  9754472
    num2 =  40   id(num2):  9755112
    num1 and num2 do not have the same identity



```python

```


---
**Score: 40**