---
draft: true
draftSectionTwo: false
created: 2024-09-19T00:00:00.000-0400
createdForSectionTwo: 2024-12-05T00:00:00.000-0400
tags: 
---

> [!NOTE]
> 
> Mr. Gordon generated this concept summary and the related exercises using ChatGPT.
> 
> He then edited the results for clarity, accuracy, and appropriate scaffolding of concepts for new programmers.

## Setup

There are many environments within which to author and run Python code.

Mr. Gordon recommends that you [[Installing Thonny|install Thonny]], if don't already have an environment within which to run Python code.

> [!TIP]
> 
> As you try out each example below, you'll likely want to save each section of code in a [[Installing Thonny#Saving a program|new Python code file]].
> 
> When you are finished these tutorials, you will have a Python code file for each example and each exercise.

## Tutorial A: Taking Input and Printing Output in Python  

In programming, **input** lets your program get data from the user, and **output** lets the program display results.

Python makes this easy with the `input()` and `print()` functions.

The `input()` function reads input from the user as a string.  

The `print()` function displays output on the screen.

---

### Lesson 1: **Simple Input and Output**  
**Concept**: Use `input()` to get user input and `print()` to display it.

#### Example 1: Greeting the User  
```python
## Ask for the user's name
name = input("What is your name? ")
print("Hello,", name + "!")  # Concatenate strings
```

#### Exercise 1: Favorite Color  
Write a program that asks the user for their favorite color and prints:  
`"Your favorite color is <color>!"`  

For example, if the user said their favourite color is green, the output would be:
`"Your favorite color is green!"`

---

### Lesson 2: **Using Numbers from User Input**  

**Concept**: Input values are strings by default, so you need to convert them to numbers for calculations using `int()` or `float()`.  

#### Example 2: Age in Five Years  
```python
## Ask the user for their age
age = int(input("How old are you? "))  # Convert input to integer
future_age = age + 5
print("In five years, you will be", future_age, "years old.")
```

#### Exercise 2: Squares
Write a program that asks the user for a number and outputs the square of that number.

---

### Lesson 3: **Formatted Output**  
**Concept**: Use `f-strings` for clean and readable output formatting.  

#### Example 3: Personalized Report Card  
```python
## Input: student name and marks
name = input("Enter your name: ")
math_marks = float(input("Enter your Math marks: "))
science_marks = float(input("Enter your Science marks: "))
average = (math_marks + science_marks) / 2

## Output: formatted string
print(f"Student Name: {name}")
print(f"Math Marks: {math_marks}")
print(f"Science Marks: {science_marks}")
print(f"Average Marks: {average:.2f}")  # Show only 2 decimal places
```

## Tutorial B: Variables and Arithmetic Operators in Python  

### Part 1: Introduction to Variables  
A **variable** is like a container that stores information. You can name the variable and use it to store values like numbers or text.  

---

#### Lesson 1: **What Are Variables?**  
**Concept**: Assigning values to variables using the `=` operator.  

##### Example 1: Storing and Using a Variable  
```python
## Storing a number in a variable
age = 15
print("I am", age, "years old.")  # Output: I am 15 years old.
```

##### Exercise 1: Personal Greeting  
Write a program that asks the user for their name and age, then prints a message like:  
`"Hello, Alice! You are 14 years old."`

---

#### Lesson 2: **Updating Variables**  
**Concept**: Variables can be updated as your program runs.  

##### Example 2: Increasing a Value  
```python
## Increase a value by 5
score = 10
score += 5  # Same as score = score + 5
print("Updated score:", score)  # Output: Updated score: 15
```

##### Exercise 2: Decreasing a value
Write a program that creates a variable and then decreases it by 11, printing the result.

---

### Part 2: Arithmetic Operators  
Python supports the following arithmetic operators:  
- `+` for addition  
- `-` for subtraction  
- `*` for multiplication  
- `/` for division (result is a float)  
- `//` for integer (floor) division  
- `%` for remainder (modulus)  
- `**` for exponentiation  

---

#### Lesson 3: **Basic Arithmetic**  
**Concept**: Using operators to perform calculations.  

##### Example 3: Simple Math  
```python
## Calculate the area of a rectangle
length = 5
width = 3
area = length * width
print("Area:", area)  # Output: Area: 15
```

##### Exercise 3a: Arithmetic Practice  
Write a program that asks the user for two numbers and performs the following operations:  
1. Addition  
2. Subtraction  
3. Multiplication  
4. Division  

##### Exercise 3b: Temperature Conversion
Write a program to store a temperature in Celsius and convert it to Fahrenheit using the formula:  
$$F = \frac{9}{5}C + 32$$

---

#### Lesson 4: **Using Multiple Operators**  
**Concept**: Combining operators to solve more complex problems.  

##### Example 4: Compound Interest  
```python
## Calculate compound interest
principal = 1000  # Initial amount
rate = 5 / 100  # Annual rate as decimal
time = 2  # Years
amount = principal * (1 + rate) ** time
print("Final amount:", amount)  # Output: Final amount: 1102.5
```

##### Exercise 4: Distance Formula  
The distance between two points $(x_1, y_1)$ and $(x_2, y_2)$ in a 2D plane is:

$$\text{distance} = \sqrt{((x_2 - x_1)^2 + (y_2 - y_1)^2)}$$  

Write a program that asks the user for the coordinates of two points and calculates the distance between them.

---

### Part 3: Applying Variables and Operators  

##### Exercise 5: Quadratic Roots  
Write a program to find the roots of a quadratic equation of the form:  

$$ax^2 + bx + c = 0$$

Use the quadratic formula:  

$$x = \frac{-b ± \sqrt{b² - 4ac}}{2a}$$  

---

## Tutorial C: Understanding Lists in Python  

*Lists* are collections of items that can store multiple values in a single variable.  

Another name for a list is an *array*.

---

### Part 1: **Creating and Accessing Lists**  

#### Lesson 1: List Basics  
**Concept**: Create a list and access its elements using indices.  

##### Example 1: Access List Elements  
```python
## Create and access a list
fruits = ["apple", "banana", "cherry"]
print(fruits[0])  # Output: apple
print(fruits[-1])  # Output: cherry (last item)
```

##### Exercise 1: Favorite Movies  
Create a list of three favorite movies and print each one on a new line.  

---

#### Lesson 2: Adding and Removing Items  
**Concept**: Use `append()` to add and `remove()` to delete items.  

##### Example 2: Grocery List  
```python
## Modify a list
groceries = ["milk", "bread"]
groceries.append("eggs")  # Add item
groceries.remove("bread")  # Remove item
print(groceries)  # Output: ['milk', 'eggs']
```

##### Exercise 2: Playlist Manager  
Create a program that lets the user add or remove songs from a playlist. Display the updated playlist after each action.

> [!TIP]
> 
> To complete this exercise, you will probably want to learn about [[Python Basics#Lesson 2 While Loops|while]] loops first.

---

### Part 2: **Iterating Through Lists**  
Use loops to process lists.  

#### Example 3: Total Prices  
```python
## Calculate the total price of items in a list
prices = [1.99, 2.49, 3.50]
total = 0
for price in prices:
    total += price
print("Total:", total)
```

#### Exercise 3: Class Scores  
Ask the user for a list of student scores. Calculate and print the class average.  

---



## Tutorial D: String Manipulation in Python  

Strings are sequences of characters. Python provides many tools to work with them.  

---

### Part 1: **Splitting Strings**  
Strings can be split into smaller parts using the `split()` method.  

#### Example 1: Split by Space  
```python
## Split a string into words
text = "10 20 30"
numbers = text.split()
print(numbers)  # Output: ['10', '20', '30']
```

#### Exercise 1: Split and Sum  
Ask the user for a series of numbers separated by spaces. Split the string and find the total sum of the numbers.  

---

### Part 2: **Joining Strings**  
Strings can be joined back together using the `join()` method.  

#### Example 2: Join Words  
```python
## Combine a list of words into a single string
words = ["hello", "world"]
sentence = " ".join(words)
print(sentence)  # Output: hello world
```

#### Exercise 2: Split Then Join
Ask the user for a sentence and print it back to them with the all of the spaces replaced by a plus sign.

For example, "It snowed yesterday" becomes "It+snowed+yesterday".  

---

## Tutorial E: Preparing for the Junior CCC (Questions 1–4)  

This tutorial will focus on teaching the core concepts needed for Questions 1 through 4 of the Junior CCC: loops, conditions, and counting. Each section builds foundational skills with examples and exercises.  

---

### Part 1: **Using Loops**  
Loops are used to repeat actions multiple times. Python has two main types: `for` and `while` loops.  

#### Lesson 1: For Loops  
**Concept**: Use `for` loops to repeat a block of code a specific number of times.  

##### Example 1: Print Numbers from 1 to 5  
```python
for i in range(1, 6):  # Range starts at 1 and ends before 6
    print(i)
```

##### Exercise 1: Multiplication Table

Write a program to print the multiplication table of a number entered by the user.  

For example, if the user enters `2`, the program would output:

```
1 x 2 = 2
2 x 2 = 4
3 x 2 = 6
4 x 2 = 8
5 x 2 = 10
6 x 2 = 12
7 x 2 = 14
8 x 2 = 16
9 x 2 = 18
10 x 2 = 20
11 x 2 = 22
12 x 2 = 24
```

---

#### Lesson 2: While Loops  
**Concept**: Use `while` loops when the number of iterations is unknown.  

##### Example 2: Sum Until Zero  
```python
## Keep summing numbers until the user enters 0
total = 0
while True:
    num = int(input("Enter a number (0 to stop): "))
    if num == 0:
        break
    total += num
print("Total:", total)
```

##### Exercise 2: Guess the Number  
Write a program where the computer comes up with a random number between 1 and 100, and the user must guess it. The program should tell the user if their guess is too high or too low and stop once they guess correctly.

For bonus achievement, tell the user how many guesses it took them to find the correct number when the game is over.

Here is how to generate a random number in Python:

```python
import random

## Generate a random integer between 1 and 100
random_number = random.randint(1, 100)
print(f"The random number is: {random_number}")
```

---

### Part 2: **Conditional Statements**  
Conditions allow the program to make decisions based on certain criteria.  

#### Lesson 1: If-Else Statements  
**Concept**: Use `if` and `else` for decision-making.  

##### Example 1: Even or Odd  
```python
## Check if a number is even or odd
num = int(input("Enter a number: "))
if num % 2 == 0:
    print("Even")
else:
    print("Odd")
```

##### Exercise 3: Pass or Fail  
Write a program that asks the user for their exam score and prints "Pass" if the score is 50 or higher, otherwise print "Fail".  

---

### Part 3: **Counting**  
Counting involves iterating through data to find matches or calculate totals.  

#### Lesson 1: Counting Characters in a String  
**Concept**: Use loops to process strings and count specific items.  

##### Example 2: Count Vowels  
```python
## Count vowels in a given string
text = input("Enter a string: ").lower()
vowels = "aeiou"
count = 0

for char in text:
    if char in vowels:
        count += 1

print("Number of vowels:", count)
```

##### Exercise 4: Count Specific Characters  
Write a program that asks the user for a string and counts how many times the letter "a" appears.  