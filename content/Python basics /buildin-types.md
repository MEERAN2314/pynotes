---
title: Buildin-Types
date: 2025-06-29
author: Your Name
cell_count: 69
score: 65
---

```python
#  Dynamic data
```


```python
#  which means we dont want to specify a data type when assigning to a variable
```


```python
#  the change in the value leads to a change in data type
```


```python
my_var = "Hi Friends!" # holding string.
my_var = 25 # same variable holding numeric value.
my_var = True #holding a boolean 
```


```python
# print(my_var)
```


```python
num1 = 10 #--> string value 
percentage = 80.50 # --> floating value
```


```python
print(num1)
print(percentage)
```

    10
    80.5



```python
#  Int Data type
```


```python
num1 = 10
num2 = 20
num3 = 30
```


```python
print(num1)
```

    10



```python
print(num2)
```

    20



```python
print(num3)
```

    30



```python
print(num1)
print(num2)
print(num3)

```

    10
    20
    30



```python
#  Floating data type

```


```python
num1 = 10.555
num2 = 20.99
```


```python
result = num1 + num2
```


```python
print(result)
```

    31.544999999999998



```python
#  Complex Data type
```


```python
num1 = 2 + 5j
num2 = 3.5 + 7.5j
```


```python
result = num1 + num2
```


```python
print(result)
```

    (5.5+12.5j)



```python
#  determine the type of variable
```


```python
num1 = 50
num2 = 20.50
```


```python
num3 = 3.5 + 7.5j
```


```python
print(type(num1))
```

    <class 'int'>



```python
print(type(num2))
```

    <class 'float'>



```python
print(type(num3))
```

    <class 'complex'>



```python
print(type(num1))
print(type(num2))
print(type(num3))
```

    <class 'int'>
    <class 'float'>
    <class 'complex'>



```python
num1 = 20
num2 = 50
```


```python
del num1
```


```python
print(num1) # --> iwll raise error because num1 deleted 
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[32], line 1
    ----> 1 print(num1) # --> iwll raise error because num1 deleted 


    NameError: name 'num1' is not defined



```python
# Boolean Data type
```


```python
a = (10 >= 4)



```


```python
b = (25 == 5 * 5)
```


```python
c = (18 != 2 * 9)
```


```python
print(a, b, c)
```

    True True False



```python
# None Data type
```


```python
a = None
```


```python
print(a)
```

    None



```python
print(type(a))
```

    <class 'NoneType'>



```python
#  String Data type
```


```python
str1 = "Hello Meeran"
```


```python
str2 = 'How are you ?'
```


```python
print(str1)
```

    Hello Meeran



```python
print(str2)
```

    How are you ?



```python
print(type(str1))
```

    <class 'str'>



```python
#  List Data type
```


```python
list = [10, 20.50, "Python", True]
```


```python
print(list)
```

    [10, 20.5, 'Python', True]



```python
print(type(list))
```

    <class 'list'>



```python
num_list = [10, 20, 30, 40]
```


```python
print(num_list)
```

    [10, 20, 30, 40]



```python
num_list[2] = 50 
```


```python
print(num_list)
```

    [10, 20, 50, 40]



```python
# Tuple Data type
```


```python
t = (10, 20, "Python", 2 + 10j)
```


```python
print(t)
```

    (10, 20, 'Python', (2+10j))



```python
print(type(t))
```

    <class 'tuple'>



```python
# Set Data type
```


```python
s = {1, 2, 'Hello', 4 + 50j}
```


```python
print(s)
```

    {'Hello', 1, 2, (4+50j)}



```python
print(type(s))
```

    <class 'set'>



```python
# Dictionary Data type
```


```python
dict = {1 : 'Orange',
        2 : 'Apple',
        3 : 'Banana'}
```


```python
print(dict)
```

    {1: 'Orange', 2: 'Apple', 3: 'Banana'}



```python
print(type(dict))
```

    <class 'dict'>



```python

```


```python

```


```python

```


---
**Score: 65**