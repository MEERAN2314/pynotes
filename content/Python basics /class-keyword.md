---
title: Class-Keyword
date: 2025-06-29
author: Your Name
cell_count: 38
score: 35
---

```python
#  class Keyword
```


```python
#  example for a class declarstion 
```


```python
class ClassExample:
    def func1(parameters):
        . . . .
    def func2(parameters):
        . . . .
```


      Cell In[3], line 3
        . . . .
        ^
    SyntaxError: invalid syntax




```python
class ClassExample:
    def func1(parameters):
        
    def func2(parameters):

        
```


      Cell In[4], line 4
        def func2(parameters):
        ^
    IndentationError: expected an indented block after function definition on line 2




```python
with open('myfile.txt', 'w') as file:
    file.write('Hi Meeran')
```


```python
#  as Keyword
```


```python
import math as x
```


```python
print(x.cos(0))
```

    1.0



```python
#  pass keyword
```


```python
def func():
    pass
class A:
    pass
```


```python
#  lambda Keyword
```


```python
cube = lambda x: x * x * x
print(cube(7))
```

    343



```python
#  import Keyword
```


```python
import math
```


```python
print(math.sqrt(25))
```

    5.0



```python
#  from Keyword
```


```python
from math import sqrt
```


```python
print(sqrt(625))
```

    25.0



```python
#  del Keyword
```


```python
my_var1 = 200
```


```python
my_var2 = "Scientech Easy"
```


```python
print(my_var1)
```

    200



```python
print(my_var2)
```

    Scientech Easy



```python
del my_var1
```


```python
del my_var2
```


```python
print(my_var1)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[27], line 1
    ----> 1 print(my_var1)


    NameError: name 'my_var1' is not defined



```python
print(my_var2)
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[28], line 1
    ----> 1 print(my_var2)


    NameError: name 'my_var2' is not defined



```python
# global Keyword
```


```python
g_var = 50
def func_read():
    print(g_var)
def func_write():
    global g_var
    g_var = 100
```


```python
func_read()
func_write()
func_read()
```

    50
    100



```python
#  nonlocal Keyword
```


```python
def outer_func():
    x = 50
    def inner_func():
        nonlocal x
        x = 100
        print("Inner function: ",x)
    inner_func()
    print("Outer function: ",x)
```


```python
outer_func()
```

    Inner function:  100
    Outer function:  100



```python
def outer_func():
    x = 50
    def inner_func():
        x = 100
        print("Inner function: ",x)
    inner_func()
    print("Outer function: ",x)
```


```python
outer_func()
```

    Inner function:  100
    Outer function:  50



```python

```


```python
outer_func()
```

    Inner function:  100
    Outer function:  50



```python

```


---
**Score: 35**