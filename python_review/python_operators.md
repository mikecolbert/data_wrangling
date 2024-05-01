# Python Operators

![Python badge](https://img.shields.io/static/v1?message=Python&logo=Python&labelColor=3776AB&color=3776AB&logoColor=white&label=%20&style=for-the-badge)  
  
## Arithmetic operators
```python
# Addition
result_addition = 5 + 3
print("Addition:", result_addition)  # Output: 8

# Subtraction
result_subtraction = 5 - 3
print("Subtraction:", result_subtraction)  # Output: 2

# Multiplication
result_multiplication = 5 * 3
print("Multiplication:", result_multiplication)  # Output: 15

# Division
result_division = 5 / 3
print("Division:", result_division)  # Output: 1.6666666666666667

# Floor Division
# Also known as integer division, it divides two numbers and returns the integer part of the result discarding any fractional part.
result_floor_division = 5 // 3
print("Floor Division:", result_floor_division)  # Output: 1

# Modulo (Remainder)
# Modulo operation returns the remainder when one number is divided by another.
result_modulus = 5 % 3
print("Modulus:", result_modulus)  # Output: 2

# Exponentiation
result_exponentiation = 5 ** 3
print("Exponentiation:", result_exponentiation)  # Output: 125
```

## Assignment operators
```python
x = 5  # Assignment
y += 2  # Increment by 2
z -= 3  # Decrement by 3
```

## Comparison operators
```python
x == y  # Equal to
x != y  # Not equal to
x > y   # Greater than
x < y   # Less than
```

## Logical operators
```python
# Logical AND
x > 0 and x < 10 # both operands must be True for statement to be True
#Logical OR
x < 0 or x > 10 # one operand must be True for the statement to be True
# Logical NOT
not (x > 0) 
```

## Membership operators
```python
x in [1, 2, 3]     # True if x is present in the list [1, 2, 3]
x not in "hello"   # True if x is not present in the string "hello"
```

