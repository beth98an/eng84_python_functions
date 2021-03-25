# Functions
### Dry - Don't repeat yourself
### What is a function and why is it useful
- Functions are reusable pieces of code that can be called using a function's name.
- Functions allow the same piece of code to be run multiple times.
- Functions break long programs up into smaller components
- Functions can be shared and used by other programmers

### How to create a function
- Syntax to create a function: def is a python keyword that tells the interpreter that the functions is being declared
- def name_of_the_function():

- Greeting function: first iteration
```
def greetings():
    print("Welcome on board")
```
- If we run this program now there will be no outcome as we have not called this function
- To call this function use`greetings()`

- Second iteration - To take the argument
```
def greetings(names):
    print("Welcome on board " + names)
```
- If we run this program now there will be no outcome as we have not called this function
- To call this function use:`greetings("James")`
- Third iteration - Create an add() to pass 2 args and adds the 2 values
```
def add(num1, num2):
    print(num1 + num2)

add(3, 2)
```
- Fourth iteration - To use return statement instead of the print()
```
def subtract(num1, num2):
    return num1 - num2
    # the return statement is the final outcome of the function

print(subtract(4, 2))
```
- Anything after the return statement does not get executed
- Create a calculator to add, subtract, divide, multiply
- Display appropriate messages with computation values as to what the outcome is from each function

```
def calculator(num1, num2):
    ad = num1 + num2
    print(f"{num1} added to {num2} is {ad}")
    sub = num1 - num2
    print(f"{num1} minus {num2} is {sub}")
    divide = num1 / num2
    print(f"{num1} divided by {num2} is {divide}")
    multi = num1 * num2
    print(f"{num1} multiplied with {num2} is {multi}")

calculator(4, 5)
```
- Create a greeting function by taking user's name and display it with the greeting message
```
def greeting(names):
    return f"Hello, {names}! How are you?"

name = input("what is your name? ")
print(greeting(name))
```