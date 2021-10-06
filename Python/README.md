### FUNCTION

#### Syntax
```Python
def function_name(parameters):
	"""docstring"""
	statement(s)

# Define function names()
def names():
    # Set up name variable with input
    name = str(input('Enter your name: '))
    # Check whether name has a vowel
    if set('aeiou').intersection(name.lower()):
        print('Your name contains a vowel.')
    else:
        print('Your name does not contain a vowel.')

    # Iterate over name
    for letter in name:
        print(letter)

# Call the function
names()
```

#### Parameters
```Python
def add_numbers(x, y, z):
    a = x + y
    b = x + z
    c = y + z
    print(a, b, c)

add_numbers(1, 2, 3)
```
or
```Python
def profile_info(username, followers):
    print("Username: " + username)
    print("Followers: " + str(followers))

# Call function with parameters assigned as above
profile_info("sammyshark", 945)

# Call function with keyword arguments
profile_info(username="AlexAnglerfish", followers=342)
```
#### Returning values
```Python
def square(x):
    y = x ** 2
    return y
result = square(3)
print(result)
```
Output: 9
```Python
def square(x):
    y = x ** 2
    # return y

result = square(3)
print(result)
```
Output: none

#### Using main as function
```Python
def hello():						
    print("Hello, World!")

def main():
    print("This is the main function.")
    hello()

main()
```
Output: 
This is main function </br>
Hello world
</br>
</br>
ex:
```Python
# Declare global variable name for use in all functions
name = str(input('Enter your name: '))

# Define function to check if name contains a vowel
def has_vowel():
    if set('aeiou').intersection(name.lower()):
        print('Your name contains a vowel.')
    else:
        print('Your name does not contain a vowel.')

# Iterate over letters in name string
def print_letters():
    for letter in name:
        print(letter)

# Define main method that calls other functions
def main():
    has_vowel()
    print_letters()


# Execute main() function
if __name__ == '__main__':
    main()
```
### Import module with dot notation
`[module].[function]`

### Aliasing
`import [module] as [another_name]`

### Call function
ex:
```
import hello # Import hello module

# Call function
hello.world()

# Print variable
print(hello.shark)
```
import math:
```Python
import math
r = math.sqrt(2)

# or

from math import sqrt
r = sqrt(2)

# or

from math import * # import everything in math
r = sqrt(2)
```
---
### Range
#### range i in python
```Python
# Example for loop
for i in [1, 2, 3, 4]:
    print(i, end=", ") # prints: 1, 2, 3, 4,

# More complex example
for i in [1, 3, 5, 7, 9]:
    x = i**2 - (i-1)*(i+1)
    print(x, end=", ") # prints 1, 1, 1, 1, 1, 
```
`range(stop)` </br>
`range(start, stop[, step])`
#### Example with two arguments
```Python
for i in range(-1, 5):
    print(i, end=", ") # prints: -1, 0, 1, 2, 3, 4, 
```
