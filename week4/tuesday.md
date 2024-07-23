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
# Let's Talk to Python: The Input Function

Hey there, young coders! Remember how we used `print()` to make Python talk to us? Well, now we're going to learn how to talk back to Python using something called the `input()` function. It's like having a conversation with your computer!

## What is the Input Function?

The `input()` function is a special tool in Python that lets us type things into our program while it's running. It's like Python is asking us a question and waiting for our answer!

Here's what it looks like:

```python
name = input("What's your name? ")
print("Nice to meet you, " + name + "!")
```

Let's break this down:

1. `input("What's your name? ")`: This part asks the question "What's your name?" and waits for you to type an answer.
2. `name = `: This stores whatever you type into a variable called `name`.
3. Then we use `print()` to say hello using the name you typed in!

## How to Use Input

Using `input()` is easy! Here are the steps:

1. Decide what question you want to ask.
2. Put that question in quotes inside the parentheses of `input()`.
3. Use a variable to save the answer.

Here's another example:

```python
favorite_color = input("What's your favorite color? ")
print("Wow, " + favorite_color + " is a great color!")
```

## Important Things to Remember

1. Python will stop and wait for you to type something and press Enter.
2. Whatever you type becomes a string (remember, that's Python's word for text).
3. If you want to use the input as a number, you need to convert it. We'll learn about that soon!

## Let's Practice!

Try making a little program that asks for two of your favorite things and then uses them in a sentence. Here's a start:

```python
food = input("What's your favorite food? ")
animal = input("What's your favorite animal? ")
print("Wow! I bet a " + animal + " would love to eat " + food + "!")
```

Now it's your turn! Can you make a program that asks for your favorite hobby and how long you've been doing it?

Remember, with `input()`, you're not just telling Python things - you're having a real back-and-forth conversation! How cool is that?
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
