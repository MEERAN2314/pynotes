---
title: Expression-Python
date: 2025-06-29
author: Your Name
cell_count: 24
score: 20
---

```python
#  Arithmetic Expression
```


```python
num1 = 20
```


```python
num2 = 40
```


```python
sum = num1 + num2 # An arithmetic expression.
```


```python
print("Sum of two numbers is ", sum)
```

    Sum of two numbers is  60



```python
num1 = 88
num2 = 22
sum = num1 + num2 # An arithmetic expression.
print("Sum of two numbers is ", sum)

```

    Sum of two numbers is  110



```python
# Relational/Conditional Expression
```


```python
num1 = int(input("Enter the first number: "))
```

    Enter the first number:  45



```python
num2 = int(input("Enter the second number: "))
```

    Enter the second number:  12



```python
num3 = int(input("Enter the third number: "))
```

    Enter the third number:  69



```python
if num1 > num2 and num1 > num3:
    print(num1, 'is a greater number among the three numbers.')
elif num2 > num1 and num2 > num3:
    print(num2, 'is a greater number among the three numbers.')
else:
    print(num3, 'is a greater number among the three numbers.')
```

    69 is a greater number among the three numbers.



```python
num1 = int(input("Enter the first number: "))
num2 = int(input("Enter the second number: "))
num3 = int(input("Enter the third number: "))

if num1 > num2 and num1 > num3:
    print(num1, 'is a greater number among the three numbers.')
elif num2 > num1 and num2 > num3:
    print(num2, 'is a greater number among the three numbers.')
else:
    print(num3, 'is a greater number among the three numbers.')

```

    Enter the first number:  67
    Enter the second number:  88
    Enter the third number:  23


    88 is a greater number among the three numbers.



```python
Age = int(input("Enter your age: "))
```

    Enter your age:  20



```python
if Age >= 18:
    print('You can cast vote.')
else:
    print('You cannot cast vote.')
```

    You can cast vote.



```python
Age = int(input("Enter your age: "))
if Age >= 18:
    print('You can cast vote.')
else:
    print('You cannot cast vote.')

```

    Enter your age:  12


    You cannot cast vote.



```python
# Logical Expression
```


```python
p = 10
```


```python
q = 15
```


```python
r = 5
```


```python
s = 20
```


```python
result = p > q and r > s
```


```python
print("Logical expression (p > q and r > s) returns ", result)
```

    Logical expression (p > q and r > s) returns  False



```python
p = 10
q = 15
r = 5
s = 20
result = p > q and r > s
print("Logical expression (p > q and r > s) returns ", result)
```

    Logical expression (p > q and r > s) returns  False



```python

```


---
**Score: 20**