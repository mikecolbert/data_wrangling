# Python Data Types

![Python badge](https://img.shields.io/static/v1?message=Python&logo=Python&labelColor=3776AB&color=3776AB&logoColor=white&label=%20&style=for-the-badge)  
  
## Int
Integer numbers without decimal points  
```python
# Define two integer variables
num1 = 10
num2 = -5

# Perform arithmetic operations
sum_result = num1 + num2
```
  
## Float
Floating-point numbers with decimal points  
```python
# Define two float variables
float1 = 3.14
float2 = -0.5

# Perform arithmetic operations
sum_result = float1 + float2
```
  
## Boolean
Boolean values representing True or False  
```python
# Define boolean variables
is_raining = True
is_sunny = False

# Perform logical operations
and_result = is_raining and is_sunny
or_result = is_raining or is_sunny
not_result = not is_raining

# Print the results
print("is_raining and is_sunny:", and_result)
print("is_raining or is_sunny:", or_result)
print("not is_raining:", not_result)
```
  
## Strings
String of characters, representing text  
```python
# Define string variables
name = "Alice"
greeting = "Hello, world!"

# Concatenate strings
full_greeting = greeting + " My name is " + name + "."
print(full_greeting)
# Hello, world! My name is Alice.
```
  
## None
Represents the absence of a value or a null value  
```python
name = None
print(name)
# None
name = "Lucy"
print(name)
# Lucy

# a function using None
def greet(name):
    if name:
        print("Hello, " + name + "!")
    else:
        print("Hello, world!")

# Call the function with and without an argument
greet("Alice")
# Hello, Alice!
greet(None)
# Hello, world!
```




