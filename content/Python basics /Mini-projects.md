---
title: Mini-Projects
date: 2025-06-29
author: Your Name
cell_count: 25
score: 25
---

```python
# Number Guessing Game
```


```python
import random

# Generate random number between 1-100
secret_number = random.randint(1, 100)
guesses = 0

print("Guess a number between 1 and 100!")
while True:
    guess = int(input("Your guess: "))
    guesses += 1
    
    if guess < secret_number:
        print("Too low!")
    elif guess > secret_number:
        print("Too high!")
    else:
        print(f"Correct! You guessed it in {guesses} tries.")
        break
```

    Guess a number between 1 and 100!


    Your guess:  6


    Too low!


    Your guess:  8


    Too low!


    Your guess:  34


    Too low!


    Your guess:  34


    Too low!


    Your guess:  2


    Too low!


    Your guess:  1


    Too low!


    Your guess:  0


    Too low!


    Your guess:  88


    Too high!


    Your guess:  77


    Too high!


    Your guess:  66


    Too high!


    Your guess:  40


    Too low!


    Your guess:  50


    Too high!


    Your guess:  48


    Too high!


    Your guess:  45


    Too low!


    Your guess:  44


    Too low!


    Your guess:  46


    Too low!


    Your guess:  47


    Correct! You guessed it in 17 tries.



```python
import random

# Generate random number between 1-100
secret_number = random.randint(1, 100)
guesses = 0

print("Guess a number between 1 and 100!")
while True:
    guess = int(input("Your guess: "))
    guesses += 1
    
    if guess < secret_number:
        print("Too low!")
    elif guess > secret_number:
        print("Too high!")
    else:
        print(f"Correct! You guessed it in {guesses} tries.")
        break
```

    Guess a number between 1 and 100!


    Your guess:  50


    Too high!


    Your guess:  30


    Too high!


    Your guess:  20


    Too high!


    Your guess:  6


    Too low!


    Your guess:  12


    Too high!


    Your guess:  10


    Too low!


    Your guess:  11


    Correct! You guessed it in 7 tries.



```python
import random

# Generate random number between 1-100
secret_number = random.randint(1, 100)
guesses = 0

print("Guess a number between 1 and 100!")
while True:
    guess = int(input("Your guess: "))
    guesses += 1
    
    if guess < secret_number:
        print("Too low!")
    elif guess > secret_number:
        print("Too high!")
    else:
        print(f"Correct! You guessed it in {guesses} tries.")
        break
        
```

    Guess a number between 1 and 100!


    Your guess:  65


    Too high!


    Your guess:  30


    Too low!


    Your guess:  2


    Too low!


    Your guess:  54


    Too low!


    Your guess:  61


    Too low!


    Your guess:  64


    Correct! You guessed it in 6 tries.



```python
# To-Do List
```


```python
todo_list = []

while True:
    print("\nTo-Do List:")
    for i, item in enumerate(todo_list, 1):
        print(f"{i}. {item}")
        
    action = input("\nAdd (a), Remove (r), or Quit (q)? ")
    
    if action == 'a':
        todo_list.append(input("Enter task: "))
    elif action == 'r':
        if todo_list:
            del todo_list[int(input("Enter task number to remove: "))-1]
    else:
        break
```

    
    To-Do List:


    
    Add (a), Remove (r), or Quit (q)?  a
    Enter task:  complete pynotes


    
    To-Do List:
    1. complete pynotes


    
    Add (a), Remove (r), or Quit (q)?  q



```python
todo_list = []

while True:
    print("\nTo-Do List:")
    for i, item in enumerate(todo_list, 1):
        print(f"{i}. {item}")
        
    action = input("\nAdd (a), Remove (r), or Quit (q)? ")
    
    if action == 'a':
        todo_list.append(input("Enter task: "))
    elif action == 'r':
        if todo_list:
            del todo_list[int(input("Enter task number to remove: "))-1]
    else:
        break
```

    
    To-Do List:


    
    Add (a), Remove (r), or Quit (q)?  q



```python
todo_list = []

while True:
    print("\nTo-Do List:")
    for i, item in enumerate(todo_list, 1):
        print(f"{i}. {item}")
        
    action = input("\nAdd (a), Remove (r), or Quit (q)? ")
    
    if action == 'a':
        todo_list.append(input("Enter task: "))
    elif action == 'r':
        if todo_list:
            del todo_list[int(input("Enter task number to remove: "))-1]
    else:
        break
```

    
    To-Do List:


    
    Add (a), Remove (r), or Quit (q)?  a
    Enter task:  complete pynotes


    
    To-Do List:
    1. complete pynotes


    
    Add (a), Remove (r), or Quit (q)?  r
    Enter task number to remove:  1


    
    To-Do List:


    
    Add (a), Remove (r), or Quit (q)?  q



```python
# Basic Calculator
```


```python
def calculator():
    print("Operations: +, -, *, /")
    num1 = float(input("First number: "))
    op = input("Operation: ")
    num2 = float(input("Second number: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        print(f"Result: {num1 / num2}")
    else:
        print("Invalid operation")

calculator()
```

    Operations: +, -, *, /


    First number:  45
    Operation:  +
    Second number:  65


    Result: 110.0



```python
def calculator():
    print("Operations: +, -, *, /")
    num1 = float(input("First number: "))
    op = input("Operation: ")
    num2 = float(input("Second number: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        print(f"Result: {num1 / num2}")
    else:
        print("Invalid operation")

calculator()
```

    Operations: +, -, *, /


    First number:  44
    Operation:  -
    Second number:  678


    Result: -634.0



```python
def calculator():
    print("Operations: +, -, *, /")
    num1 = float(input("First number: "))
    op = input("Operation: ")
    num2 = float(input("Second number: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        print(f"Result: {num1 / num2}")
    else:
        print("Invalid operation")

calculator()
```

    Operations: +, -, *, /


    First number:  234
    Operation:  65
    Second number:  34


    Invalid operation



```python
def calculator():
    print("Operations: +, -, *, /")
    num1 = float(input("First number: "))
    op = input("Operation: ")
    num2 = float(input("Second number: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        print(f"Result: {num1 / num2}")
    else:
        print("Invalid operation")

calculator()
```

    Operations: +, -, *, /


    First number:  34
    Operation:  *
    Second number:  56


    Result: 1904.0



```python
def calculator():
    print("Operations: +, -, *, /")
    num1 = float(input("First number: "))
    op = input("Operation: ")
    num2 = float(input("Second number: "))
    
    if op == '+':
        print(f"Result: {num1 + num2}")
    elif op == '-':
        print(f"Result: {num1 - num2}")
    elif op == '*':
        print(f"Result: {num1 * num2}")
    elif op == '/':
        print(f"Result: {num1 / num2}")
    else:
        print("Invalid operation")

calculator()
```

    Operations: +, -, *, /


    First number:  34
    Operation:  /
    Second number:  2


    Result: 17.0



```python
# Password Generator
```


```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: LZtsA8SGP6Om



```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: IuwZlqJ@02rr



```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: 8f%1KvjDMLDP



```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: $r5I^@nscq5Y
    Your new password: s0RWg*YYMSLY



```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: 7&fBMvQU^dqT



```python
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
import random
import string

def generate_password(length=12):
    chars = string.ascii_letters + string.digits + "!@#$%^&*"
    password = ''.join(random.choice(chars) for _ in range(length))
    return password

print("Your new password:", generate_password())
```

    Your new password: nBpytoP4^TR3
    Your new password: fY%Vi1TEb&6A
    Your new password: p*II4d^DvIBi
    Your new password: I!TyvV^1rB0g



```python
# Countdown Timer
```


```python
import time

def countdown(seconds):
    while seconds:
        mins, secs = divmod(seconds, 60)
        print(f"{mins:02d}:{secs:02d}", end="\r")
        time.sleep(1)
        seconds -= 1
    print("Time's up!")

countdown(60)  # 1 minute countdown
```

    Time's up!



```python

```


```python

```


---
**Score: 25**