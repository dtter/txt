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
> [More](https://github.com/dtter/txt/blob/master/Python/functiong-and-import-module/function.md)
### Import module with dot notation
`[module].[function]`

### Aliasing
`import [module] as [another_name]`
> [More](https://github.com/dtter/txt/blob/master/Python/functiong-and-import-module/import.md)
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
