# Python Lesson 2: Making Choices with If-Else

## Let's Get Started
We'll use the same website as before to write our Python code. [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what decision trees are
2. Use if-else to make choices in Python
3. Make a program that responds differently based on what you type

## Part 1: What are Decision Trees?

Sometimes, we want our code to make choices. A decision tree is like a map that helps the computer decide what to do.

## Part 2: If-Else Statements

In Python, we use if-else to make choices. Here's how it looks:

```python
if something is true:
    # do this
else:
    # do that instead
```

Let's see an example:

```python
age = 12

if age >= 13:
    print("You can ride the big roller coaster!")
else:
    print("Sorry, you're too young for this ride.")
```

In this example, if the age is 13 or more, it says one thing. If not, it says something else.

### Your Turn:
1. Make a variable called `temperature` and give it a number.
2. Write an if-else that says "It's hot!" if the temperature is above 30, and "It's cool." if it's not.

## Part 3: Adding More Choices with Elif

Sometimes we want more than two choices. We can use `elif` (short for "else if") to add more:

```python
weather = "rainy"

if weather == "sunny":
    print("Don't forget your sunglasses!")
elif weather == "rainy":
    print("Bring an umbrella!")
else:
    print("Enjoy your day!")
```

This code checks for different types of weather and says something different for each.

### Your Turn:
1. Make a variable called `favorite_fruit` and give it a fruit name.
2. Write an if-elif-else that says something different for at least three fruits, and something else for any other fruit.

## Let's Make: A Mini Adventure Game

Let's make a simple adventure game using if-else. Here's how:

1. Ask the player to choose a direction ("left", "right", or "forward").
2. Use if-elif-else to tell them what happens based on their choice.

Here's how to start:

```python
print("You're on a quest and reach a fork in the road.")
choice = input("Do you go left, right, or forward? ")

if choice == "left":
    print("You find a treasure chest!")
elif choice == "right":
    print("You meet a friendly dragon!")
elif choice == "forward":
    print("You discover a hidden cave!")
else:
    print("Oops! You got lost.")
```

Now, make your own adventure game with at least three choices and different things happening for each!

## Great Job!
You've finished your second Python lesson! You learned how to use if-else to make choices in your code. Next time, we'll learn about loops and how to do things over and over in Python!