---
title: Funct-Arg
date: 2025-06-30
author: Your Name
cell_count: 40
score: 40
---

```python
# Default Arguments in Python
```


```python
def studentInfo(name, gender = 'Male'):
```


      Cell In[2], line 1
        def studentInfo(name, gender = 'Male'):
                                               ^
    SyntaxError: incomplete input




```python
def studentInfo(name, gender = 'Male'):
# This function displays the student's info passed in the function parameters.
    print('Name:',name)
    print('Gender:',gender)
```


```python
# Main program.
```


```python
# Function call 1.
```


```python
studentInfo('Deepak')
```

    Name: Deepak
    Gender: Male



```python
# Function call 2.
```


```python
studentInfo('Tripti', gender = 'Female')
```

    Name: Tripti
    Gender: Female



```python
def studentInfo(name, rollNo = 20, branch = 'Electrical'):
    print('Name:',name,'Roll no:',rollNo,'Branch:',branch)
```


```python
# Main program.
```


```python
# Function call 1.
```


```python
studentInfo(name = 'John')
```

    Name: John Roll no: 20 Branch: Electrical



```python
# Function call 2.
```


```python
studentInfo(name = 'Bob', rollNo = 10)
```

    Name: Bob Roll no: 10 Branch: Electrical



```python
# Function call 3.
```


```python
studentInfo(name = 'Jenny', rollNo = 5, branch = 'Computer Science')
```

    Name: Jenny Roll no: 5 Branch: Computer Science



```python
# Required Arguments in Python
```


```python

# example error code
```


```python
# Program to find the area and perimeter of rectangle using function required arguments.

```


```python
def rectangle(length, breadth):
    areaRec = length * breadth # Area of rectangle.
    perRec = 2 * (length + breadth) # Perimeter of rectangle.
    print("Area of rectangle = ",areaRec)
    print("Perimeter of rectangle = ",perRec)
```


```python
# Main program.
```


```python
def main():
    ln = int(input("Enter the length of rectangle: "))
    br = int(input("Enter the breadth of rectangle: "))
    rectangle(ln) # Intentionaly missing one argument value.
```


```python
main() # function calling.
```

    Enter the length of rectangle:  43
    Enter the breadth of rectangle:  43



    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[23], line 1
    ----> 1 main() # function calling.


    Cell In[22], line 4, in main()
          2 ln = int(input("Enter the length of rectangle: "))
          3 br = int(input("Enter the breadth of rectangle: "))
    ----> 4 rectangle(ln)


    TypeError: rectangle() missing 1 required positional argument: 'breadth'



```python
# Keyword Arguments in Python
```


```python
# Displaying persons info.
```


```python
def display(name, age, gender):
    print('Name:',name)
    print('Age:',age)
    print('Gender:',gender)
```


```python
def main():
 # First function call.
    display('John', 20, 'M') # function calling from another function.
 # Second function call.
    display('Jenny', 18, 'F')
```


```python
main() # function calling.
```

    Name: John
    Age: 20
    Gender: M
    Name: Jenny
    Age: 18
    Gender: F



```python
# Displaying persons info.
```


```python
def display(name, age, gender):
    print('Name:',name)
    print('Age:',age)
    print('Gender:',gender)
def main():
  # First function call.
    display('Herry', age = 20, gender = 'M') # function calling from another function.
  # Second function call.
    display(age = 18, gender = 'F', name = 'Jimmy')
main() # function calling.
```

    Name: Herry
    Age: 20
    Gender: M
    Name: Jimmy
    Age: 18
    Gender: F



```python
# Variable length Arguments
```


```python
# args is the name of variable length parameters.
```


```python
def my_function(*args):
    "function docstring"
    # body of the function
    return [expression]
```


```python
# Example 1:
```


```python
# Function definition with variable length parameters. 

```


```python
def my_function(*args): # Here, args is name of formal parameter.
    print(args)
print('Calling function with two arguments')
my_function(10, 20)

print('Calling function with three arguments')
my_function(10, 20, 30)
print('Calling function with four arguments')
my_function(20, 30, 40, 50)
```

    Calling function with two arguments
    (10, 20)
    Calling function with three arguments
    (10, 20, 30)
    Calling function with four arguments
    (20, 30, 40, 50)



```python
# Function definition with one formal parameter and variable length parameters.

```


```python
def listDay(arg1, *arg2):
    print(arg1, arg2, sep="")
def main():
    listDay('Name of days are:', 'Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
main() # function calling.
```

    Name of days are:('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')



```python
def listDay(arg1, *arg2):
    print(arg1, arg2, sep="")
def main():
    listDay('Name of days are:', 'Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')
main() # function calling.
```

    Name of days are:('Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday')



```python

```


---
**Score: 40**