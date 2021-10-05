# Learning_Python
(Based on the learning currently going through)
# Hello World

```python
print("Hello World")
```

# The Print Function

```python
print("   /|")
print("  / |")
print(" /  |")
print("/___|")
```

# Variables

```python
print("My name is Shripad")
print("I am 60 years old")
print("I like my name Shripad a lot")
print("But I don't like being 60")

# Updating variables would be a hectic task

character_name = "Shripad"
character_age = "60"
print("My name is " + character_name + ",")
print("I am 60 "+ character_age + " years old")
print("I like my name " + character_name + " a lot")
print("But I don't like being " + character_name)

character_name = "Shripad" # String variable
character_age = 59.6 # Integer/Float variable
is_female = False # Boolean variable
```

# Strings

```python
print("IIT Madras")
print("IIT\nMadras") # Newline operator
print("IIT\"Madras") # Using the backslash
print("IIT\Madras")

phrase = "IIT Madras" 
print(phrase) # Printing a string

print(phrase + " is amazing") # Using comcatenation operator

print(phrase.lower()) # Converts all to lowercase
print(phrase.upper()) # Converts all to uppercase
print(phrase.isupper()) # Checks if everything is uppercase
print(phrase.upper().isupper()) # Converts, then checks

print(len(phrase)) # Prints length of the string

print(phrase[0]) # Prints character at given index
print(phrase[3])

print(phrase.index("M")) # Prints inde of given character
print(phrase.index("Mad"))
print(phrase.index("z")) # Error

print(phrase.replace("Madras", "Bombay") # Replaces part of a string

```

# Numbers

```python
print(2)
print(2.89)
print(-6.88)

print(3 + 4.5) # Addition operator

print(3 * 4 + 5) # Preserves order of operation
print(3 * (4 + 5))

print(10 % 3) # Remainder operator

num = 5
print(num)
print(str(num) + "My fav number") # Printing with strings

print(abs(num)) # Prints absolute value
print(pow(3, 2)) # Raises first number to the power of the second number 
print(max(3, 2)) # Prints out maximum of the two numbers
print(min(3, 2))
print(round(3.2)) # Rounds off the number
print(round(3.7))

from math import * # To import special functions

print(floor(7.8)) # Prints floor integer
print(ceil(7.8)) # Prints ceiling integer
print(sqrt(36)) # Prints square root of the nymber
```

# Inputs

```python
name = input("Enter your name: ")
age = input("Enter your age: ")
print("Hello " + name + "! You are" + age)
```

# Activity - Building a Basic Calculator

```python
num1 = input("Enter a number: ")
num2 = input("Enter another number: ")

result = num1 + num2 # Error
print(result)

result = int(num1) + int(num2)
result = float(num1) + float(num2)
```

# Activity - Creating a Mad Libs Game

```python
print("Roses are red")
print("Violets are blue")
print("I love you")

colour = input("Enter a colour: ")
plural_noun = input("Enter a plural noun: ")
sportsman = input("Enter a sportsman: ")

print("Roses are {colour}") # Pseudocode
print("{plural noun} are blue")
print("I love {sportsman}")

print("Roses are " + colour)
print(plural noun + " are blue")
print("I love " + sportsman)
```

# Lists

```python
friends = ["Aakash", "Ramesh", "Harsh", "Rocky", "Aditya"]
friends_1 = ["Aakash", 2, False]

print(friends)
print(friends[1]) # Prints the second element
print(friends[-1]) # Prints the last element
print(friends[1:3]) # Prints the second to third element
```

# List Functions

```python
num = [11, 23, 11, 23, 77, 89, 08]
friends = ["Aakash", "Ramesh", "Harsh", "Rocky", "Aditya"]

print(friends) # Prints the list

friends.extend(num) # Appends given list at the end 
friends.extend("Parth") # Appends given element at the end

friends.insert(1, "Divya") # Adds given element at given index

friends.remove("Ramesh") # Removes given element from the list
friends.clear() # Empties the list
friends.pop() # Removes last element

print(friends.index("Harsh")) # Prints index of element
print(friends.count("Rocky")) # Prints number of occurances

friends.sort() # Sorts the list
num.reverse() # Reverses the list

new_friends = friends.copy() # Copies the list
```

# Tuples

```python
coordinates = (2, 3) # Immutable
print(coordinates[1]) # Print an item with index  

coord = [(2, 3), (3, 4), (5, 7)] # A list of tuples
# Lists are mutable, tuples aren't
```

# Functions

```python
def say_hello(): # Defining a function
	print("Hello everyone")

say_hello() # Calling a function

def say_hi(name): # Taking a parameter
	print("Hello "+ name)

say_hi("Parth")
```

# Return Statement

```python
def cube(num):
	return (num**3) 
	# No code can be put after the return statement

print(cube(3))

result = cube(4)
print(result)
```

# If Statements

```python
is_male = True

if is_male:
	print("Hey man!")
else:
	print("Hello lady!")

is_tall = False
is_male = True

if is_male or is_tall:
	do_something()
if is_male and is_tall:
	do_something()

elif is_male and not (is_tall):
	do_something()
```

# If statements and Comparisons

```python
def max_num(num1, num2, num3):
	if num1 >= num2 and num1 >= num3:
		return num1
	elif num2 >= num1 and num2 >= num3:
		return num2
	else:
		return num3

print(max_num(300,40,5))

num1 >= num2 # Greater than or equal to
num1 <= num2 # Lesser than or equal to
num1 == num2 # Equal to
num1 > num2 # Greater than
num1 < num2 # Lesser than
```

# Activity : Building a Better Calculator

```python
num1 = float(input("Enter first number: "))
operator = input("Enter operator: ")
num2 = float(input("Enter second number: "))

if op == "+":
	print(num1 + num2)
elif op == "-":
	print(num1 - num2)
elif op == "*":
	print(num1 * num2)
elif op == "/":
	print(num1 / num2)
else:
	print("Invalid oparator")
```

# Dictionaries

```python
months = {
	"Jan": "January",
	"Feb": "February",
	"Mar": "March",
}

print(months["Mar"])
print(months.get("Dec"))

print(months.get("Fun", "Not a valid key")) # We can give a default value using .get()
```
