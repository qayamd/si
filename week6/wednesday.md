# Python Lesson 3: Fun with Loops and Comparisons

## Let's Get Started
Remember our coding playground? [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what comparison operators are and how to use them
2. Use `for` loops to do things over and over
3. Use `while` loops to keep doing something until we say stop
4. Use `break` and `continue` to control our loops

## Part 1: Comparison Operators

Before we jump into loops, let's learn about comparison operators. These are special symbols that help us compare things in Python. They're like the "greater than" and "less than" signs you use in math!

Here are the main comparison operators:

- `==` means "is equal to"
- `!=` means "is not equal to"
- `<` means "is less than"
- `>` means "is greater than"
- `<=` means "is less than or equal to"
- `>=` means "is greater than or equal to"

Let's see some examples:

```python
print(5 == 5)  # This will print True
print(5 != 3)  # This will print True
print(5 < 10)  # This will print True
print(5 > 10)  # This will print False
print(5 <= 5)  # This will print True
print(5 >= 10) # This will print False
```

We use these operators to make decisions in our code. They always give us a True or False answer.

## Part 2: What are Loops?

Now that we know how to compare things, let's learn about loops! Imagine you have to write your name five times. You could do this:

```python
print("Alex")
print("Alex")
print("Alex")
print("Alex")
print("Alex")
```

That's a lot of typing! Loops let us tell the computer to do something many times without writing it over and over.

## Part 3: For Loops

A `for` loop is like a helper that does something a certain number of times. Here's how it looks:

```python
for i in range(5):
    print("Hello!")
```

This will say "Hello!" five times. Let's break it down:

- `for` tells Python we're starting a loop
- `i` is a variable that changes each time the loop runs
- `in range(5)` tells Python to run the loop 5 times
- The indented line(s) after the `:` is what Python will do each time

### Your Turn:
1. Write a for loop that counts from 1 to 5.
   Pseudocode:
   ```
   Use a for loop with range()
   Inside the loop, print the current number
   ```
   Hint: You can use `range(1, 6)` to count from 1 to 5.

2. Make a for loop that says your name three times.
   Pseudocode:
   ```
   Use a for loop that repeats 3 times
   Inside the loop, print your name
   ```
   Hint: You can use `range(3)` to repeat something 3 times.

## Part 4: While Loops

A `while` loop keeps doing something as long as a condition is true. It's like saying "keep going until I say stop!"

Here's an example:

```python
count = 0
while count < 5:
    print(count)
    count = count + 1
```

This will count from 0 to 4. Let's break it down:

- `while` tells Python to keep looping while something is true
- `count < 5` is the condition. It uses the "less than" operator (`<`) we learned earlier. The loop runs as long as this is true
- The indented lines run each time through the loop
- `count = count + 1` increases the count each time, so we eventually stop

### Your Turn:
1. Write a while loop that counts down from 5 to 1.
   Pseudocode:
   ```
   Set a variable 'count' to 5
   While count is greater than 0:
       Print count
       Decrease count by 1
   ```
   Hint: Use `>` to check if count is greater than 0.

2. Make a while loop that asks someone to guess a secret word, and keeps asking until they guess right.
   Pseudocode:
   ```
   Set a variable 'secret_word' to your chosen word
   Set a variable 'guess' to an empty string
   While guess is not equal to secret_word:
       Ask for a guess and store it in 'guess'
       If guess is correct, print a success message
   ```
   Hint: Use `!=` to check if the guess is not equal to the secret word.

## Part 5: Controlling Loops with Break and Continue

Sometimes we want to have more control over our loops. That's where `break` and `continue` come in!

### Break

`break` lets us exit a loop early. It's like saying "Stop everything and get out of the loop!"

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

This will only print numbers 0 to 4, because when `i` becomes equal to (`==`) 5, we break out of the loop.

### Continue

`continue` lets us skip the rest of the current loop and move to the next one. It's like saying "Skip this, go to the next!"

```python
for i in range(5):
    if i == 2:
        continue
    print(i)
```

This will print 0, 1, 3, 4, skipping 2 because of the `continue`.

### Your Turn:
1. Make a loop that prints numbers from 0 to 10, but stops when it reaches 7.
   Pseudocode:
   ```
   Use a for loop to iterate from 0 to 10
   Inside the loop:
       If the number equals 7:
           Break out of the loop
       Print the number
   ```
   Hint: Use `==` to check when to break.

2. Create a loop that prints all numbers from 0 to 5, except for the number 3.
   Pseudocode:
   ```
   Use a for loop to iterate from 0 to 5
   Inside the loop:
       If the number equals 3:
           Continue to the next iteration
       Print the number
   ```
   Hint: Use `==` to check when to continue.

## Let's Make: A Number Guessing Game

Let's use everything we've learned to make a fun number guessing game!

```python
secret_number = 7
guess = 0

while guess != secret_number:
    guess = int(input("Guess the number (1-10): "))
    if guess < secret_number:
        print("Too low! Try again.")
    elif guess > secret_number:
        print("Too high! Try again.")

print("You got it! The number was", secret_number)
```

In this game:
- We use `!=` to check if the guess is not equal to the secret number
- We use `<` to check if the guess is too low
- We use `>` to check if the guess is too high

Can you add a counter to tell the player how many guesses they took?

## Great Job!
You've mastered loops and comparisons in Python! You can now make your programs do things over and over and make decisions based on comparisons. Next time, we'll learn about lists and how to work with groups of things in Python!
