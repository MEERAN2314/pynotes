---
title: Comparison-Operator
date: 2025-06-29
author: Your Name
cell_count: 90
score: 90
---

```python
#  Comparison  Operators
```


```python
# Equal to (==)
```


```python
x = 20
y = 20
```


```python
print( x == y)
```

    True



```python
p = 'My name is John'
q = 'My name is John'
```


```python
print( p == q)
```

    True



```python
r = 'Text'
s = 'text'
```


```python
print( r == s)
```

    False



```python
t = [1, 2, 3, 4]
u = [1, 2, 3]
```


```python
print( t == u)
```

    False



```python
List1 = [10, 20, 30, 40, 50]
```


```python
List2 = List1
```


```python
print( List1 == List2)
```

    True



```python
x = 50.0
y = 50
```


```python
print(x == y)
```

    True



```python
str1 = 'My name is John'
```


```python
str2 = str1
```


```python
print(str1 == str2)
```

    True



```python
a = True
```


```python
b = 1
```


```python
print(a == b)
```

    True



```python
#   Not equal to (!=)
```


```python
x = 50
y = 90

```


```python
print( x != y)
```

    True



```python
str1 = 'My name is John'
```


```python
str2 = str1
```


```python
print( str1 != str2)
```

    False



```python
a = True
```


```python
b = 1

```


```python
print( a != b)
```

    False



```python
p = False
```


```python
q = 0
```


```python
print( p != q)
```

    False



```python
r = '50'
s = 50
```


```python
print( r != s)
```

    True



```python
r = 50
s = 50
```


```python
print( r != s)
```

    False



```python
List1 = [10, 20, 'Python', '30']
List2 = [10, 20, 'Python', 30]
```


```python
print(List1 != List2)
```

    True



```python
List1 = [10, 20, 'Python', 30]
List2 = [10, 20, 'Python', 30]
```


```python
print(List1 != List2)
```

    False



```python
Dict1 = {
     1: 'a',
     2: '20'
}
Dict2 = {
    1: 'a',
    2: '20'
}
```


```python
print(Dict1 != Dict2)
```

    False



```python
#  Greater than (>)
```


```python
num1 = 60
num2 = 50
```


```python
print(num1 > num2)
```

    True



```python
print(num1 + 20 - 20 > num2 + 20)
```

    False



```python
n1 = 20
n2 = n1
```


```python
print(n1 > n2)
```

    False



```python
str1 = 'Python' # --> considered by len
str2 = 'Pythe'
```


```python
print(str1 > str2)
```

    True



```python
str1 = 'Python' #--> different data type will raise a error 
str2 = '20'
```


```python
print(str1 > str2)

```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[56], line 1
    ----> 1 print(str1 > str2)


    TypeError: '>' not supported between instances of 'str' and 'int'



```python
str1 = 'Python'
str2 = '20'
print(str1 > str2)
```

    True



```python
p = True
q = 2
```


```python
print(q > p)
```

    True



```python
r = False
s = -1
```


```python
print(r > s)
```

    True



```python
List1 = [10, 20, 30]
List2 = [10, 20, 40]
```


```python
print(List1 > List2)
```

    False



```python
#  Less than (<)
```


```python
num1 = 20
num2 = 20.05
```


```python
print(num1 < num2)
```

    True



```python
exp1 = 20 * 20 % 20
exp2 = 20 + 20 / 20
```


```python
print(exp2 < exp1)
```

    False



```python
str1 = 'Python'
str2 = 'Text'
```


```python
print(str1 < str2)
```

    True



```python
r = False
s = -2
```


```python
print(r < s)
```

    False



```python
List1 = [1, 2, 3]
List2 = [1, 2, 4]
```


```python
print(List1 < List2)
```

    True



```python
# Greater than or equal to (>=)
```


```python
num1 = 20.20
num2 = 20.0200
```


```python
print(num1 >= num2)
```

    True



```python
x = True + 2
y = False + False + False
```


```python
print(x >= y)
```

    True



```python
p = 'abcd'
q = 'abcde'
```


```python

print(p >= q)
```

    False



```python
#  Less than or equal to (<=)
```


```python
num1 = 40.40
num2 = 40.400
```


```python
print(num1 <= num2)
```

    True



```python
x = True + 2
y = False + False + False
```


```python
print(x <= y)
```

    False



```python
p = 'A'
q = 'B'
```


```python
print(p <= q)
```

    True



```python
# Use of Comparison Operators in Decision Making Statement
```


```python
# Program to illustrate the use of comparison or relational operators.
```


```python
p = 50
q = 60
if(p == q):
    print("p is equal to q")
else:
    print("p is not equal to q")
if(p != q):
    print("p is not equal to q")
else:
    print("p is equal to q")
if(p > q):
    print("p is greater than q")
else:
    print("p is not greater than q")
if(p < q): print("p is less than q") 
else: 
    print("p is not less than q")
if(p >= q):
    print("p is greater than or equal to q")
else:
    print("p is not greater than or equal to q")
if(p <= q):
    print("p is less than or equal to q")
else:
    print("p is not less than or equal to q")
```

    p is not equal to q
    p is not equal to q
    p is not greater than q
    p is less than q
    p is not greater than or equal to q
    p is less than or equal to q



```python
age = int(input("Enter your age: "))
if(age >= 18):
    print("You are eligible for voting.")
else:
    print("You are not eligible for voting.")
```

    Enter your age:  20


    You are eligible for voting.



```python

```


---
**Score: 90**