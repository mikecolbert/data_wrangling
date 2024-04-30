# Python Data Structures
[Lists](#lists)
[Tuples](#tuples)
[Dictionaries](#dictionaries})
## [Lists]
- Square brackets []
- Mutable data structure  
- Can contain same or different data types and even sub-lists  

### Creating lists
```python
list_0 = [] # empty list
list_1 = ["dog", "cat", "hamster"]
list_2 = [1, 2.01, 5, 6.7]
list_3 = [["dog", 24], ["cat", 5], "hamster", 0]

# A list containing dictionaries
fruit_list = [{"apple":12,"banana":8},{"cherry":1, "blueberry":4}]
    
# A list containing tuples
fruit_list = [("apple", 12),("banana", 8),("cherry",1),("blueberry",4)]
```

### Accessing list elements with indices
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

### List methods

```python
# Append element to th end of the list
lst.append("apple")
# ['apple', 'banana', 'cherry', 'blueberry', 'apple']

# Insert an element at a specific index position in the list
lst.insert("cherry", 1)
# ['apple', 'cherry', 'banana', 'cherry', 'blueberry', 'apple']

# Count the number of occurences of an element value in the list
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
  
## (Tuples)
- Parens ()
- Immutable data structure (cannot be changed after creation)
- Faster than lists
- Can contain same or different data types 

### Creating tuples
```python
tuple_1 = ("dog", "cat", "hamster")
tuple_2 = (1, 2.01, 5, "pig")

# A list containing dictionaries
fruit_list = [{"apple":12,"banana":8},{"cherry":1, "blueberry":4}]
    
# A list containing tuples
fruit_list = [("apple", 12),("banana", 8),("cherry",1),("blueberry",4)]

# Convert a string to tuple
fruit = "apple"
fruit_tuple = tuple(fruit)

# Convert a list to tuple
fruit_list = ['apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry']
fruit_tuple = tuple(fruit_list)    

# Convert a set to tuple
set_1 = {5,6,7,8}
numeric_tuple = tuple(set_1)
```
### Accessing tuple elements with indices
```python
fruit_tuple = ('apple', 'banana', 'blueberry', 'banana', 'cherry', 'cherry')

# Get the length of the tuple
len(fruit_tuple)
# 6

# Delete a tuple
del(fruit_tuple)

# Tuple indices (zero indexing)
fruit_tuple[0]
# 'apple'
fruit_tuple[2]
# 'blueberry'

# Negative tuple indices
fruit_tuple[-1]  # last element in the tuple
# 'cherry'

fruit_tuple[-2:] # the last two elements in the tuple
# ('cherry', 'cherry')

fruit_tuple[:-2] # everything except the last two elements in the tuple
# ('apple', 'banana', 'blueberry', 'banana')

# [start_index (inclusive) : end_index (exclusive)]
# The slice will include the start_index, and everything until but excluding the end_index
fruit_tuple[0:3]
# ('apple', 'banana', 'blueberry')
```

### Tuple methods
```python
# Count the number of occurences of an element in the tuple
fruit_tuple.count('cherry')
# 2

# Return the position (index) of the first occurance of an element in the tuple
fruit_tuple.index('banana')
# 1
```
## {Dictionaries}
- curly braces {}
- Mutable data structure
- Ordered in Python >3.6 (can refer to index)
- key:value pairs
- Cannot have duplicate keys
- Can contain same or different data types 
- Keys must be immutable data types (strings, numbers, tuples)
- Values can be any data type - string, integer, a list, another dictionary, boolean, etc.

### Creating dictionaries
```python
# Create an empty dictionary
vehicles = dict()
print(vehicles)
# {}

# Create a dictionary
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99}
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}

# Create a dictionary with various data types
# Notice "engine" key has a value that is another dictionary
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99, "engine":{"cylinders": 8, "hybrid": True}}
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'engine': {'cylinders': 8, 'hybrid': True}}

### convert tuple to dictionary
### convert list to dictionary
```
### Accessing dictionary elements
```python
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99, "engine":{"cylinders": 8, "hybrid": True}}
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'engine': {'cylinders': 8, 'hybrid': True}}

# Access value by key name
print(vehicles["price"])
# 25999.99

# "hybrid" key inside of "engine" key
print(vehicles["engine"]["hybrid"])
# True

# vehicles is a five element dictionary.
len(vehicles)
# 5

# there is a two element dictionary inside of the "engine" key.
len(vehicles["engine"])
# 2

# Delete a dictionary
del(vehicles)
```

### Dictionary use cases
```python
# Create a list of dictionaries
vehicles = [{"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99, "engine":{"cylinders": 8, "hybrid": True}}]

# Append a new dictionary to the list
new_vehicle = {"make":"Chevy", "model":"Tahoe", "year":2022, "price": 35999, "engine":{"cylinders": 8, "hybrid": False}}
vehicles.append(new_vehicle)

print(vehicles)
[{'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'engine': {'cylinders': 8, 'hybrid': True}}, 
{'make': 'Chevy', 'model': 'Tahoe', 'year': 2022, 'price': 35999, 'engine': {'cylinders': 8, 'hybrid': False}}]
```


### Dictionary methods
```python
# Returns a copy of the dictionary
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99}
vehicles_2 = vehicles.copy()
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}
print(vehicles_2)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}

# Removes all the elements from a dictionary
vehicles_2.clear()
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}
print(vehicles_2)
# {}

# Returns the value of the specified key. If the key does not exist: insert the key, with the specified value
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99}
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}
vehicles.setdefault("lot","A") # "lot" key doesn't exist so it is added
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'lot': 'A'}
vehicles.setdefault("model", "test") # "model" key exists so it is returned
# Explorer

# Returns a dictionary with the specified keys and value
keys = ( "key_1", "key_2", "key_3")
values = 0
new_dict = dict.fromkeys(keys, values)
print(new_dict)
# {'key_1': 0, 'key_2': 0, 'key_3': 0}

# Returns the value of a specified key
print(vehicles.get("year"))
# 2019

# Returns a list containing a tuple for each key value pair
print(vehicles.items())
# dict_items([('make', 'Ford'), ('model', 'Explorer'), ('year', 2019), ('price', 25999.99), ('trim_level', 'sport')]

# Returns a list of dictionary keys
vehicles.keys()
# dict_keys(['make', 'model', 'year', 'price', 'engine'])

# Removes the element with the specified key
vehicles = {"make":"Ford", "model":"Explorer", "year":2018, "price": 25999.99, "engine":{"cylinders": 8, "hybrid": True}}
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'engine': {'cylinders': 8, 'hybrid': True}}
vehicles.pop("engine")
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}

# Removes the last inserted key value pair
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99, 'color': 'gray'}
vehicles.popitem()
print(vehicles)
{'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}

# Updates the dictionary with the new specified key-value pairs
print(vehicles)
# {'make': 'Ford', 'model': 'Explorer', 'year': 2018, 'price': 25999.99}
vehicles.update({"year": 2019, "trim_level":"sport"}) # pass parameter as a dictionary, updates existing value, adds new key:value
print(vehicles)
 # {'make': 'Ford', 'model': 'Explorer', 'year': 2019, 'price': 25999.99, 'trim_level': 'sport'}

# Returns a list of dictionary values
vehicles.values()
# dict_values(['Ford', 'Explorer', 2018, 25999.99, {'cylinders': 8, 'hybrid': True}])
```

## Set

#queue
#stack/dequeue
https://www.geeksforgeeks.org/stack-and-queues-in-python/





