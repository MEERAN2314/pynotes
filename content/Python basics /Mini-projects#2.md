---
title: Mini-Projects#2
date: 2025-06-29
author: Your Name
cell_count: 26
score: 25
---

```python
#  Basic Hangman Game
```


```python
import random

words = ["python", "jupyter", "notebook", "programming"]
word = random.choice(words)
guessed = ["_"] * len(word)
tries = 6

while tries > 0 and "_" in guessed:
    print(" ".join(guessed))
    guess = input("Guess a letter: ").lower()
    
    if guess in word:
        for i, letter in enumerate(word):
            if letter == guess:
                guessed[i] = guess
    else:
        tries -= 1
        print(f"Wrong! {tries} tries left.")

print("You won!" if "_" not in guessed else "You lost! Word was: " + word)
```

    _ _ _ _ _ _


    Guess a letter:  notebook


    Wrong! 5 tries left.
    _ _ _ _ _ _


    Guess a letter:  jupyter


    Wrong! 4 tries left.
    _ _ _ _ _ _


    Guess a letter:  python


    _ _ _ _ _ _


    Guess a letter:  programming


    Wrong! 3 tries left.
    _ _ _ _ _ _


    Guess a letter:  python


    _ _ _ _ _ _


    Guess a letter:  jupyter


    Wrong! 2 tries left.
    _ _ _ _ _ _


    Guess a letter:  jupyter


    Wrong! 1 tries left.
    _ _ _ _ _ _


    Guess a letter:  jupyter


    Wrong! 0 tries left.
    You lost! Word was: python



```python
import random

words = ["python", "jupyter", "notebook", "programming"]
word = random.choice(words)
guessed = ["_"] * len(word)
tries = 6

while tries > 0 and "_" in guessed:
    print(" ".join(guessed))
    guess = input("Guess a letter: ").lower()
    
    if guess in word:
        for i, letter in enumerate(word):
            if letter == guess:
                guessed[i] = guess
    else:
        tries -= 1
        print(f"Wrong! {tries} tries left.")

print("You won!" if "_" not in guessed else "You lost! Word was: " + word)
```

    _ _ _ _ _ _ _ _ _ _ _


    Guess a letter:  sd


    Wrong! 5 tries left.
    _ _ _ _ _ _ _ _ _ _ _


    Guess a letter:  sd


    Wrong! 4 tries left.
    _ _ _ _ _ _ _ _ _ _ _


    Guess a letter:  a


    _ _ _ _ _ a _ _ _ _ _


    Guess a letter:  w


    Wrong! 3 tries left.
    _ _ _ _ _ a _ _ _ _ _


    Guess a letter:  t


    Wrong! 2 tries left.
    _ _ _ _ _ a _ _ _ _ _


    Guess a letter:  yt


    Wrong! 1 tries left.
    _ _ _ _ _ a _ _ _ _ _


    Guess a letter:  python


    Wrong! 0 tries left.
    You lost! Word was: programming



```python
# Temperature Converter
```


```python
def temp_converter():
    print("1. Celsius to Fahrenheit")
    print("2. Fahrenheit to Celsius")
    choice = int(input("Choose conversion (1/2): "))
    
    if choice == 1:
        c = float(input("Enter Celsius: "))
        print(f"{c}°C = {(c * 9/5) + 32}°F")
    else:
        f = float(input("Enter Fahrenheit: "))
        print(f"{f}°F = {(f - 32) * 5/9}°C")

temp_converter()
```

    1. Celsius to Fahrenheit
    2. Fahrenheit to Celsius


    Choose conversion (1/2):  1
    Enter Celsius:  30


    30.0°C = 86.0°F



```python
def temp_converter():
    print("1. Celsius to Fahrenheit")
    print("2. Fahrenheit to Celsius")
    choice = int(input("Choose conversion (1/2): "))
    
    if choice == 1:
        c = float(input("Enter Celsius: "))
        print(f"{c}°C = {(c * 9/5) + 32}°F")
    else:
        f = float(input("Enter Fahrenheit: "))
        print(f"{f}°F = {(f - 32) * 5/9}°C")

temp_converter()
```

    1. Celsius to Fahrenheit
    2. Fahrenheit to Celsius


    Choose conversion (1/2):  2
    Enter Fahrenheit:  120


    120.0°F = 48.888888888888886°C



```python
def temp_converter():
    print("1. Celsius to Fahrenheit")
    print("2. Fahrenheit to Celsius")
    choice = int(input("Choose conversion (1/2): "))
    
    if choice == 1:
        c = float(input("Enter Celsius: "))
        print(f"{c}°C = {(c * 9/5) + 32}°F")
    else:
        f = float(input("Enter Fahrenheit: "))
        print(f"{f}°F = {(f - 32) * 5/9}°C")

temp_converter()
```

    1. Celsius to Fahrenheit
    2. Fahrenheit to Celsius


    Choose conversion (1/2):  1
    Enter Celsius:  54


    54.0°C = 129.2°F



```python
def temp_converter():
    print("1. Celsius to Fahrenheit")
    print("2. Fahrenheit to Celsius")
    choice = int(input("Choose conversion (1/2): "))
    
    if choice == 1:
        c = float(input("Enter Celsius: "))
        print(f"{c}°C = {(c * 9/5) + 32}°F")
    else:
        f = float(input("Enter Fahrenheit: "))
        print(f"{f}°F = {(f - 32) * 5/9}°C")

temp_converter()
```

    1. Celsius to Fahrenheit
    2. Fahrenheit to Celsius


    Choose conversion (1/2):  2
    Enter Fahrenheit:  99


    99.0°F = 37.22222222222222°C



```python
# Basic Web Scraper
```


```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

print("Page Title:", soup.title.text)
print("\nAll links:")
for link in soup.find_all('a'):
    print(link.get('href'))
```

    Page Title: Example Domain
    
    All links:
    https://www.iana.org/domains/example



```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

print("Page Title:", soup.title.text)
print("\nAll links:")
for link in soup.find_all('a'):
    print(link.get('href'))
```

    Page Title: Example Domain
    
    All links:
    https://www.iana.org/domains/example



```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

print("Page Title:", soup.title.text)
print("\nAll links:")
for link in soup.find_all('a'):
    print(link.get('href'))
```

    Page Title: Example Domain
    
    All links:
    https://www.iana.org/domains/example



```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

print("Page Title:", soup.title.text)
print("\nAll links:")
for link in soup.find_all('a'):
    print(link.get('href'))
```

    Page Title: Example Domain
    
    All links:
    https://www.iana.org/domains/example



```python
import requests
from bs4 import BeautifulSoup

url = "https://example.com"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')

print("Page Title:", soup.title.text)
print("\nAll links:")
for link in soup.find_all('a'):
    print(link.get('href'))
```

    Page Title: Example Domain
    
    All links:
    https://www.iana.org/domains/example



```python
# Dice Rolling Simulator
```


```python
import random

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
```

    You rolled: 1


    Roll again? (y/n)  y


    You rolled: 3


    Roll again? (y/n)  n



```python
import random

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
```

    You rolled: 1


    Roll again? (y/n)  n



```python
import random

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
```

    You rolled: 5


    Roll again? (y/n)  n



```python
import random

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
```

    You rolled: 2


    Roll again? (y/n)  n



```python
import random

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
```

    You rolled: 1


    Roll again? (y/n)  y


    You rolled: 6


    Roll again? (y/n)  n



```python
import randomy

def roll_dice():
    return random.randint(1, 6)

while True:
    print("You rolled:", roll_dice())
    if input("Roll again? (y/n) ").lower() != 'y':
        break
        
```

    You rolled: 3


    Roll again? (y/n)  y


    You rolled: 5


    Roll again? (y/n)  y


    You rolled: 5


    Roll again? (y/n)  y


    You rolled: 2


    Roll again? (y/n)  y


    You rolled: 2


    Roll again? (y/n)  y


    You rolled: 4


    Roll again? (y/n)  y


    You rolled: 1


    Roll again? (y/n)  n



```python
# BMI Calculator
```


```python
def calculate_bmi():
    weight = float(input("Enter weight (kg): "))
    height = float(input("Enter height (m): "))
    bmi = weight / (height ** 2)
    
    print(f"Your BMI: {bmi:.1f}")
    if bmi < 18.5:
        print("Underweight")
    elif 18.5 <= bmi < 25:
        print("Normal weight")
    else:
        print("Overweight")

calculate_bmi()
```

    Enter weight (kg):  45
    Enter height (m):  180


    Your BMI: 0.0
    Underweight



```python
def calculate_bmi():
    weight = float(input("Enter weight (kg): "))
    height = float(input("Enter height (m): "))
    bmi = weight / (height ** 2)
    
    print(f"Your BMI: {bmi:.1f}")
    if bmi < 18.5:
        print("Underweight")
    elif 18.5 <= bmi < 25:
        print("Normal weight")
    else:
        print("Overweight")

calculate_bmi()
```

    Enter weight (kg):  61
    Enter height (m):  180


    Your BMI: 0.0
    Underweight



```python
def calculate_bmi():
    weight = float(input("Enter weight (kg): "))
    height = float(input("Enter height (m): "))
    bmi = weight / (height ** 2)
    
    print(f"Your BMI: {bmi:.1f}")
    if bmi < 18.5:
        print("Underweight")
    elif 18.5 <= bmi < 25:
        print("Normal weight")
    else:
        print("Overweight")

calculate_bmi()
```

    Enter weight (kg):  100
    Enter height (m):  140


    Your BMI: 0.0
    Underweight



```python

```


---
**Score: 25**