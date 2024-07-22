# Python Lesson 3: Fun with Loops

## Let's Get Started
We'll use the same website as before to write our Python code. [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what loops are and why they're cool
2. Use `for` loops to do things over and over
3. Use `while` loops to keep doing something until we say stop

## Part 1: What are Loops?

Loops let us tell the computer to do something many times. They're great when we want to do the same thing over and over without writing it again and again.

## Part 2: For Loops

A `for` loop is like a helper that does something a certain number of times. Here's how it looks:

```python
for i in range(5):
    print("Hello!")
```

This will say "Hello!" five times. The `range(5)` tells Python to count from 0 to 4.

### Your Turn:
1. Write a for loop that counts from 1 to 5.
2. Make a for loop that says your name three times.

## Part 3: While Loops

A `while` loop keeps doing something as long as we tell it to. It's like saying "keep going until I say stop!"

Here's an example:

```python
count = 0
while count < 5:
    print(count)
    count = count + 1
```

This will count from 0 to 4. The loop keeps going as long as `count` is less than 5.

### Your Turn:
1. Write a while loop that counts down from 5 to 1.
2. Make a while loop that asks someone to guess a secret word, and keeps asking until they guess right.

## Let's Make: A Number Guessing Game

Let's make a fun game where you guess a secret number. Here's how:

1. Pick a secret number and remember it.
2. Use a while loop to keep asking for guesses.
3. Use if-else to give hints (too high or too low).
4. Stop the loop when they guess the right number.

Here's how to start:

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

Now, make your own number guessing game. Can you add a counter to tell the player how many guesses they took?

## Great Job!
You've finished your third Python lesson! You learned how to use for loops and while loops to do things over and over in your code. Next time, we'll learn about lists and how to work with groups of things in Python!