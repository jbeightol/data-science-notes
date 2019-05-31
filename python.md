# Python

## Lesson Objectives

1. Print a message
1. Add a comment
1. Create a variable and assign it a value
1. Explain the different data types
1. Perform calculations with variables
1. Use string operations
1. Create a list
1. Access an element of a list
1. Perform a set of commands depending on a situation
1. Get user input
1. Repeatedly perform a set of commands
1. Use a for loop
1. Create a class for an object

## Print a message

You can print a message to the user

```python
print "hello!"
```

## Add a comment

- Comments let you summarize what you're doing
- They don't get executed

```python
# this will not be executed
```

## Create a variable and assign it a value

```python
a = "hello"
print a ##print the value of the variable 'a'
```

## Explain the different data types

There are lots of different types of data that you can use in python

- String (text)
- Integers (whole numbers)
- Float (decimal numbers)
- Booleans (True/False)

You can convert one data type to another

```python
a = str(1) #a = "1"
b = int("5") #b = 5
c = float(4) #c = 4.0
d = int(5.7) #d = 5
```

## Perform calculations with variables

```python
a = 1
b = a + 1 #b = 2
c = b * 3 #c = 6
d = c - 1 #d = 5
e = float(d) / 2 #e = 2.5
f = d ** 2 #exponent: f = 25
```

## Use string operations

```python
a = "first string"
b = "second string"
c = a + " " + b
```

## Create a list

You can create lists of things

```python
a = [1, 5, "some string", True, 5.6]
```

You can even have lists of lists

```python
a = [
    [1, 2, 3], #first row
    [4, 5, 6], #second row
    [7, 8, 9], #third row
    [10] #fourth row
]
```

You can conceptualize a list of lists however you want

### ACTIVITY

How would you change the previous example so that each inner list is a column?

## Access an element of a list

Lists have elements stored at numerical indexes, starting at 0

```python
a = [1, 5, "some string", True, 5.6]
print a[0] #1
print a[1] #5
print a[4] #5.6
```

## Perform a set of commands depending on a situation

```python
a = 22
if a < 10:
    print "a is less than 10"
elif a == 10:
    print "a is 10"
else:
    print "a is greater than 10"
```

The conditions can be

- `<` less than
- `>` greater than
- `<=` less than or equal to
- `>=` greater than or equal to
- `==` an exact match

You can also compare strings:

```python
a = 'oh hai!'
if a == 'oh hai!':
    print 'this works'
```

## Get user input

You can get user input from the command like so:

```python
user_input = raw_input("Please enter something: ")
print "you entered: " + user_input
```



### ACTIVITY

Write a program that models this flow chart:

![where should I post that?](http://socialnewsdaily.com/wp-content/uploads/2013/04/where-do-i-post-it.jpg)

## Repeatedly perform a set of commands

```python
a = 10
while a < 20:
    print "the value of a is currently: " + str(a)
    a = a + 1
```

### ACTIVITIES

1. Write a program that models this flow chart:

    ![pictionary](../images/pictionary.jpeg)

1. Given the following list [70, 95, 97, 55, 3, 24, 89, 97, 84, 11]
    - Write a program that loops through each value in the list and prints it
    - Write a program that loops through each value in the list and adds them all together
    - Write a program that loops through each value in the list and prints the average
    - Write a program that loops through each value in the list and prints the minimum
    - Write a program that loops through each value in the list and prints the maximum
1. Combine all the programs from the previous step into one program that asks the user what operation they would like to do
1. Alter the last program so that it performs the operations for only numbers that are greater than a number specified by the user



## Excercise 

Ben has a very simple idea to make some profit: he buys something and sells it again. Of course, this wouldn't give him any profit at all if he was simply to buy and sell it at the same price. Instead, he's going to buy it for the lowest possible price and sell it at the highest.

Write a function that returns both the minimum and maximum number of the given list/array.

### example

```python
min_max([1,2,3,4,5])   == [1,5]
```

## Use a for loop

The process of looping through an array can be simplified with a `for` loop:

```python
foods = ['hot dogs', 'beer', 'bald eagles']
for food in foods:
      print(food)
```

The `for loop` allows you to perform a repetitive task on every element within an object, such as every every name in a list.


Lets see how the sudo code works

```python
# for each individual object in the list
    # perform task_A on said object
    # once task_A has been completed, move to next object in the list
```

Lets say we wanted to print each of the names in the list and as well as 'Is Awesome!'


### ACTIVITIES

### Write a `for`-loop that iterates from the number 1 to the number 15.

On each iteration, print out the number.


### Iterate from 1 to 15, printing whether the number is odd or even.

Hint: The modulus operator, `%`, can be used to take the remainder. For example:

```python
9 % 5 == 4
```

Or in other words, the remainder of dividing 9 by 5 is 4. 

### Iterate through the following list of animals, and print each one in all caps.

```python
animals = ['duck', 'rat', 'boar', 'slug', 'mammoth', 'gazelle']
```

### Iterate through the animals list. Capitalize the first letter and append the modified animals to a new list.


<a id='fizz_buzz'></a>
### Iterate from 1 to 30 with the following instructions:

1. If a number is divisible by 3, print 'fizz'. 
2. If a number is divisible by 5, print 'buzz'. 
3. If a number is both divisible by 3 and 5 print 'fizzbuzz'.
4. Otherwise, print just the number.

<a id='functions'></a>


### 3s and 5s

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.



### Finding the Hypotenuse 

Create a function that takes the two shorter sides of a right triangle and returns the hypotenuse 



# Functions
---

Similar to the way we can use for loops as a means of performing repetitive tasks on a series of objects we can create functions to perform repetitve tasks as well.  The use behind a function is that we can write a large block of actions within a function and then call the function whenever we want to use it.  


Lets make some sudo code.
```python
# define the function name and the requirements it needs
    # perform actions
    # optional : return output
```

Lets create a function at takes two numbers as arguments and returns their sum, difference and product. 


### Write a function to calculate the area of a triangle uaing a height and width.

Test it out.



## Create a class for an object

You can use a `class` or blueprint for objects that you'll use

```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def greet(self):
    print("Hello, my name is " + self.name + ". My age is " + str(self.age))

me = Person("Matt", 36)
me.greet()
sally = Person("Sally", 53)
sally.greet()
```

- `__init__` is a function that gets called when a new object is created.
- `self` is the object that's created

