
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
