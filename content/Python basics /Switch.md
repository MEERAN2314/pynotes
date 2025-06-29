---
title: Switch
date: 2025-06-30
author: Your Name
cell_count: 31
score: 30
---

```python
# Switch Statement in Python

```


```python
city = 'd' # Initialize the variable.
if city == 'm':
    print('Mumbai')
elif city == 'd':
    print('Dhanbad')
elif city == 'c':
    print('Chennai')
elif city == 'r':
    print('Ranchi')
else:
    print('No city')
```

    Dhanbad



```python
# Implementing Switch Statement in Python using Dictionary
```


```python
# Implementing switch case statement in Python using Dictionary.
```


```python
def m():
    return "Mumbai"
def d():
    return "Dhanbad"
def c():
    return "Chennai"
def r():
    return "Ranchi"
def default():
    return "No city"
```


```python
# Creating a dictionary and put these in it.
```


```python
switcher = {
    1: m,
    2: d,
    3: c,
    4: r,
    }
```


```python
# Creating a function named switch with a parameter.
```


```python
def switch(city):
    return switcher.get(city, default)()
print(switch(1)) # Calling function.
print(switch(2)) # Calling function.
```

    Mumbai
    Dhanbad



```python
# Program to create a simple calculator by implementing switch case statement in Python using Dictionary.
```


```python
x = int(input('Enter your first number: '))
y = int(input('Enter your second number: '))
choice = int(input('Enter your choice 1: addition 2: subtraction 3: Multiplication and 4: division: '))
def addition():
    sum = x + y
    return sum
def subtraction():
    sub = x - y
    return sub
def multiplication():
    multiply = x * y
    return multiply
def division():
    div = x / y
    return div
def default():
    return "You are not entered the valid choice."

# Putting these in the dictionary.
switcher = {
    1: addition,
    2: subtraction,
    3: multiplication,
    4: division,
    }
def switch(number):
    return switcher.get(number, default)()
print(switch(choice))
```

    Enter your first number:  69
    Enter your second number:  88
    Enter your choice 1: addition 2: subtraction 3: Multiplication and 4: division:  4


    0.7840909090909091



```python
# Implementing Switch Statement using Python Class
```


```python
# Creating a class.
```


```python
class PythonSwitch():
    def main_function(self, name_of_day):
        default = "Incorrect name of day"
        method_name = 'day_' + str(name_of_day)
        method = getattr(self, method_name, lambda: default())
        return method()

    def day_1(self):
        return "Sunday"
    def day_2(self):
        return "Monday"
    def day_3(self):
        return "Tuesday"

    def day_4(self):
        return "Wednesday"
    def day_5(self):
        return "Thursday"
    def day_6(self):
        return "Friday"
    def day_7(self):
        return "Saturday"
```


```python
# Creating an object of class.
```


```python
my_switch = PythonSwitch()
print(my_switch.main_function(1)) # Calling function with passing argument value.
print(my_switch.main_function(3)) # Calling function.
```

    Sunday
    Tuesday



```python
# Implementing Switch Case using Functions and Lambdas
```


```python
def a():
    return 'Apple'
def m():
    return 'Mango'
def o():
    return 'Orange'
```


```python
def fruits(i):
    switcher = {
        1: a,
        2: m,
        3: o,
        4: lambda: 'Banana'
    }
    funct = switcher.get(i, lambda: 'Invalid')
    return funct()
```


```python
print(fruits(3)) # Calling function.
print(fruits(0)) # Calling function.
```

    Orange
    Invalid



```python
# Implement Switch Statement with match and case in Python 3.10
```


```python
# This program code will execute only in python 3.10 or above versions
```


```python
lang = input('Which programming language do you want to learn? ')

match lang:
    case "JavaScript":
        print('You will be a web developer after learning JavaScript.')

    case "Python":
        print("You will be a Data Scientist after learning Python.")

    case "PHP":
        print("You will be a backend developer after learning PHP.")

    case "Solidity":
        print("You will be a Blockchain developer after learning Solidity.")

    case "Java":
        print("You will be a software developer after learning Java")
    case _:
        print("Language does not matter.")
```

    Which programming language do you want to learn?  java


    Language does not matter.



```python
lang = input('Which programming language do you want to learn? ')

match lang:
    case "JavaScript":
        print('You will be a web developer after learning JavaScript.')

    case "Python":
        print("You will be a Data Scientist after learning Python.")

    case "PHP":
        print("You will be a backend developer after learning PHP.")

    case "Solidity":
        print("You will be a Blockchain developer after learning Solidity.")

    case "Java":
        print("You will be a software developer after learning Java")
    case _:
        print("Language does not matter.")
```

    Which programming language do you want to learn?  python


    Language does not matter.



```python
lang = input('Which programming language do you want to learn? ')

match lang:
    case "JavaScript":
        print('You will be a web developer after learning JavaScript.')

    case "Python":
        print("You will be a Data Scientist after learning Python.")

    case "PHP":
        print("You will be a backend developer after learning PHP.")

    case "Solidity":
        print("You will be a Blockchain developer after learning Solidity.")

    case "Java":
        print("You will be a software developer after learning Java")
    case _:
        print("Language does not matter.")
```

    Which programming language do you want to learn?  Python


    You will be a Data Scientist after learning Python.



```python
lang = input('Which programming language do you want to learn? ')

match lang:
    case "JavaScript":
        print('You will be a web developer after learning JavaScript.')

    case "Python":
        print("You will be a Data Scientist after learning Python.")

    case "PHP":
        print("You will be a backend developer after learning PHP.")

    case "Solidity":
        print("You will be a Blockchain developer after learning Solidity.")

    case "Java":
        print("You will be a software developer after learning Java")
    case _:
        print("Language does not matter.")
```

    Which programming language do you want to learn?  Java


    You will be a software developer after learning Java



```python
lang = input('Which programming language do you want to learn? ')

match lang:
    case "JavaScript":
        print('You will be a web developer after learning JavaScript.')

    case "Python":
        print("You will be a Data Scientist after learning Python.")

    case "PHP":
        print("You will be a backend developer after learning PHP.")

    case "Solidity":
        print("You will be a Blockchain developer after learning Solidity.")

    case "Java":
        print("You will be a software developer after learning Java")
    case _:
        print("Language does not matter.")
```

    Which programming language do you want to learn?  JavaScript


    You will be a web developer after learning JavaScript.



```python
choice = int(2)
match choice:
    case 1:
        print('You chose 1')
    case 2:
        print('You chose 2')
    case 3:
        print('You chose 3')
    case _:
        print('Default option')
```

    You chose 2



```python
choice = int()
match choice:
    case 1:
        print('You chose 1')
    case 2:
        print('You chose 2')
    case 3:
        print('You chose 3')
    case _:
        print('Default option')
```

    Default option



```python
choice = int(3)
match choice:
    case 1:
        print('You chose 1')
    case 2:
        print('You chose 2')
    case 3:
        print('You chose 3')
    case _:
        print('Default option')
```

    You chose 3



```python

```


---
**Score: 30**