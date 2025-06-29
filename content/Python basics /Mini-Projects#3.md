---
title: Mini-Projects#3
date: 2025-06-30
author: Your Name
cell_count: 26
score: 25
---

```python
# Mad Libs Generator
```


```python
# Mad Libs - Fill in the blanks story generator
print("Welcome to Mad Libs!")
noun = input("Enter a noun: ")
verb = input("Enter a verb: ")
adjective = input("Enter an adjective: ")
place = input("Enter a place: ")

story = f"Yesterday, I saw a {adjective} {noun} {verb} at {place}. It was amazing!"
print("\nYour Mad Lib:")
print(story)
```

    Welcome to Mad Libs!


    Enter a noun:  car
    Enter a verb:  at
    Enter an adjective:  intersting
    Enter a place:  beach


    
    Your Mad Lib:
    Yesterday, I saw a intersting car at at beach. It was amazing!



```python
# Mad Libs - Fill in the blanks story generator
print("Welcome to Mad Libs!")
noun = input("Enter a noun: ")
verb = input("Enter a verb: ")
adjective = input("Enter an adjective: ")
place = input("Enter a place: ")

story = f"Yesterday, I saw a {adjective} {noun} {verb} at {place}. It was amazing!"
print("\nYour Mad Lib:")
print(story)
```

    Welcome to Mad Libs!


    Enter a noun:  ball
    Enter a verb:  is
    Enter an adjective:  forgot
    Enter a place:  park


    
    Your Mad Lib:
    Yesterday, I saw a forgot ball is at park. It was amazing!



```python
# Rock-Paper-Scissors Game
```


```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  rock


    
    You: rock
    Computer: paper
    Computer wins!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  scissors


    
    You: scissors
    Computer: scissors
    Tie!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  paper


    
    You: paper
    Computer: rock
    You win!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  paper


    
    You: paper
    Computer: scissors
    Computer wins!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  paper


    
    You: paper
    Computer: paper
    Tie!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  paper


    
    You: paper
    Computer: paper
    Tie!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  paper


    
    You: paper
    Computer: scissors
    Computer wins!



```python
import random

choices = ["rock", "paper", "scissors"]
user = input("Choose (rock/paper/scissors): ").lower()
computer = random.choice(choices)

print(f"\nYou: {user}\nComputer: {computer}")

if user == computer:
    print("Tie!")
elif (user == "rock" and computer == "scissors") or \
     (user == "paper" and computer == "rock") or \
     (user == "scissors" and computer == "paper"):
    print("You win!")
else:
    print("Computer wins!")
```

    Choose (rock/paper/scissors):  rock


    
    You: rock
    Computer: scissors
    You win!



```python
#  Fibonacci Sequence Generator 
```


```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms"""
    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]

terms = int(input("How many Fibonacci terms? "))
print(f"First {terms} terms:", fibonacci(terms))
```

    How many Fibonacci terms?  12


    First 12 terms: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]



```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms"""
    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]

terms = int(input("How many Fibonacci terms? "))
print(f"First {terms} terms:", fibonacci(terms))
```

    How many Fibonacci terms?  50


    First 50 terms: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, 10946, 17711, 28657, 46368, 75025, 121393, 196418, 317811, 514229, 832040, 1346269, 2178309, 3524578, 5702887, 9227465, 14930352, 24157817, 39088169, 63245986, 102334155, 165580141, 267914296, 433494437, 701408733, 1134903170, 1836311903, 2971215073, 4807526976, 7778742049]



```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms"""
    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]

terms = int(input("How many Fibonacci terms? "))
print(f"First {terms} terms:", fibonacci(terms))
```

    How many Fibonacci terms?  99


    First 99 terms: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181, 6765, 10946, 17711, 28657, 46368, 75025, 121393, 196418, 317811, 514229, 832040, 1346269, 2178309, 3524578, 5702887, 9227465, 14930352, 24157817, 39088169, 63245986, 102334155, 165580141, 267914296, 433494437, 701408733, 1134903170, 1836311903, 2971215073, 4807526976, 7778742049, 12586269025, 20365011074, 32951280099, 53316291173, 86267571272, 139583862445, 225851433717, 365435296162, 591286729879, 956722026041, 1548008755920, 2504730781961, 4052739537881, 6557470319842, 10610209857723, 17167680177565, 27777890035288, 44945570212853, 72723460248141, 117669030460994, 190392490709135, 308061521170129, 498454011879264, 806515533049393, 1304969544928657, 2111485077978050, 3416454622906707, 5527939700884757, 8944394323791464, 14472334024676221, 23416728348467685, 37889062373143906, 61305790721611591, 99194853094755497, 160500643816367088, 259695496911122585, 420196140727489673, 679891637638612258, 1100087778366101931, 1779979416004714189, 2880067194370816120, 4660046610375530309, 7540113804746346429, 12200160415121876738, 19740274219868223167, 31940434634990099905, 51680708854858323072, 83621143489848422977, 135301852344706746049]



```python
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms"""
    sequence = [0, 1]
    while len(sequence) < n:
        sequence.append(sequence[-1] + sequence[-2])
    return sequence[:n]

terms = int(input("How many Fibonacci terms? "))
print(f"First {terms} terms:", fibonacci(terms))
```

    How many Fibonacci terms?  3


    First 3 terms: [0, 1, 1]



```python
# Palindrome Checker 
```


```python
def is_palindrome(word):
    """Check if word reads the same forwards and backwards"""
    cleaned = word.lower().replace(" ", "")
    return cleaned == cleaned[::-1]

text = input("Enter a word/phrase: ")
print(f"'{text}' is {'a palindrome' if is_palindrome(text) else 'not a palindrome'}")
```

    Enter a word/phrase:  hello meeran


    'hello meeran' is not a palindrome



```python
def is_palindrome(word):
    """Check if word reads the same forwards and backwards"""
    cleaned = word.lower().replace(" ", "")
    return cleaned == cleaned[::-1]

text = input("Enter a word/phrase: ")
print(f"'{text}' is {'a palindrome' if is_palindrome(text) else 'not a palindrome'}")
```

    Enter a word/phrase:  markram


    'markram' is a palindrome



```python
def is_palindrome(word):
    """Check if word reads the same forwards and backwards"""
    cleaned = word.lower().replace(" ", "")
    return cleaned == cleaned[::-1]

text = input("Enter a word/phrase: ")
print(f"'{text}' is {'a palindrome' if is_palindrome(text) else 'not a palindrome'}")
```

    Enter a word/phrase:  fool


    'fool' is not a palindrome



```python
# Currency Converter (Using Fixed Rates)
```


```python
rates = {'USD': 1.0, 'EUR': 0.85, 'GBP': 0.75, 'JPY': 110.0}

amount = float(input("Enter amount: "))
from_curr = input("From currency (USD/EUR/GBP/JPY): ").upper()
to_curr = input("To currency (USD/EUR/GBP/JPY): ").upper()

result = amount * rates[to_curr] / rates[from_curr]
print(f"{amount} {from_curr} = {result:.2f} {to_curr}")
```

    Enter amount:  450
    From currency (USD/EUR/GBP/JPY):  USD
    To currency (USD/EUR/GBP/JPY):  EUR


    450.0 USD = 382.50 EUR



```python
rates = {'USD': 1.0, 'EUR': 0.85, 'GBP': 0.75, 'JPY': 110.0}

amount = float(input("Enter amount: "))
from_curr = input("From currency (USD/EUR/GBP/JPY): ").upper()
to_curr = input("To currency (USD/EUR/GBP/JPY): ").upper()

result = amount * rates[to_curr] / rates[from_curr]
print(f"{amount} {from_curr} = {result:.2f} {to_curr}")
```

    Enter amount:  2
    From currency (USD/EUR/GBP/JPY):  EUR
    To currency (USD/EUR/GBP/JPY):  GBP


    2.0 EUR = 1.76 GBP



```python
rates = {'USD': 1.0, 'EUR': 0.85, 'GBP': 0.75, 'JPY': 110.0}

amount = float(input("Enter amount: "))
from_curr = input("From currency (USD/EUR/GBP/JPY): ").upper()
to_curr = input("To currency (USD/EUR/GBP/JPY): ").upper()

result = amount * rates[to_curr] / rates[from_curr]
print(f"{amount} {from_curr} = {result:.2f} {to_curr}")
```

    Enter amount:  44
    From currency (USD/EUR/GBP/JPY):  JPY
    To currency (USD/EUR/GBP/JPY):  USD


    44.0 JPY = 0.40 USD



```python

```


---
**Score: 25**