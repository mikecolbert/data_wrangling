# Data Wrangling
## Python Data Types
### Boolean
### Integer
### Float
### Strings

## Python Data Structures
### Lists
- Square brackets []
- Mutable data structure  
- Can contain same or different data types and even sub-lists  

#### Creating lists
```python
list_0 = [] # empty list
list_1 = ["dog", "cat", "hamster"]
list_2 = [1, 2.01, 5, 6.7]
list_3 = [["dog", 24], ["cat", 5], "hamster", 0]
```

#### Accessing list elements with indices
```python
# Create list
lst = ["apple", "banana", "cherry", "blueberry"]
print(lst)
# ['apple', 'banana', 'cherry', 'blueberry']

# Get the length of the list
len(lst)
# 4

# Delete a list
del(lst)

# List indices (zero indexing)
lst[0]
# 'apple'
lst[2]
# 'cherry'

# Negative list indices
lst[-1]  # last element in the list
# 'blueberry'

lst[-2:] # last two elements in the list
# ['cherry', 'blueberry']

lst[:-2] # first two elements in the list
# ['apple', 'banana']

# Getting sublists with slicing
# [start_index (inclusive) : end_index (exclusive)]
# The slice will include the start_index, and everything until but excluding the end_index
lst = ["apple", "banana", "cherry", "blueberry"]
print(lst[0])
# apple
print(lst[2])
# cherry
print(lst[0:2])
['apple', 'banana']

# Accessing sub-lists with indexing
list_3 = [["dog", 24], ["cat", 5], "hamster", 0]
print(list_3[0])
# ['dog', 24]
print(list_3[0][1]) # in the root list get the zero index, in the sub-list ge the 1 index
# 24
print(list_3[2])
hamster
```

#### List methods

```python
# Append element to th end of the list
lst.append("apple")
# ['apple', 'banana', 'cherry', 'blueberry', 'apple']

# Insert an element at a specific index position in the list
lst.insert("cherry", 1)
# ['apple', 'cherry', 'banana', 'cherry', 'blueberry', 'apple']

# Count the number of occurences of an element in the list
lst.count("apple")
# 2

# Remove and return the last element in the list
pop_value = lst.pop()
print(pop_value)
# apple
print(lst)
# ['apple', 'cherry', 'banana', 'cherry', 'blueberry']

# Sort elements in the list in ascending order
lst.sort()
print(lst)
# ['apple', 'banana', 'blueberry', 'cherry', 'cherry']

# Reverse the order of elements in the list
lst.reverse()
print(lst)
# ['cherry', 'cherry', 'blueberry', 'banana', 'apple']

# Remove and returns the first occurance of an element in the list
lst = ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
lst.remove('banana')
print(lst)
# ['apple', 'blueberry', 'banana', 'cherry', 'cherry']

# Return the position (index) of the first occurance of an element in the list
lst = ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
lst.index('banana')
# 1

# Return a copy of the list
lst = ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
lst2 = lst.copy()
print(lst2)
# ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']

# Add all elements of an iterable (another list) to a list
lst = ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
lst3 = ["mushrooms", "lemon", "orange"]

print(lst)
# ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
print(lst3)
# ['mushrooms', 'lemon', 'orange']

lst.extend(lst3)
print(lst)
# ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry', 'mushrooms', 'lemon', 'orange']

# Remove all elements from the list
lst3 = ["mushrooms", "lemon", "orange"]
print(lst3)
# ['mushrooms', 'lemon', 'orange']

lst3.clear()
print(lst3)
# []
```


### Dictionary
### Tuple
### Set

#queue
#stack/dequeue
https://www.geeksforgeeks.org/stack-and-queues-in-python/





