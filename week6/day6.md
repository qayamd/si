# Python Lesson 6: Fun with Functions

## Let's Get Started
Remember our coding playground? <a href="https://www.programiz.com/python-programming/online-compiler/" target="_blank">Click here to open it</a>

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what functions are and why they're useful
2. Create your own simple functions
3. Use functions with parameters

## Part 1: What are Functions?

Functions are like special helpers in your program. They're sets of instructions that you can use over and over again. Think of them as magic spells that do specific jobs for you!

## Part 2: Creating Simple Functions

Here's how we make a simple function:

```python
def say_hello():
    print("Hello, friend!")

# Now let's use our function
say_hello()
```

Let's break this down:
- `def` tells Python we're creating a function
- `say_hello()` is the name we gave our function
- The indented line is what our function does
- To use the function, we write its name followed by parentheses

### Your Turn:
1. Create a function called `sing_chorus()` that prints out your favorite line from a song.
2. Use your function three times to sing the chorus!

## Part 3: Functions with Parameters

We can make our functions more flexible by giving them parameters. These are like ingredients we can give to our function:

```python
def greet(name):
    print("Hello, " + name + "!")

# Now let's use our function
greet("Alex")
greet("Sam")
```

### Your Turn:
1. Make a function called `draw_shape(shape)` that prints "I'm drawing a " followed by whatever shape you tell it.
2. Use your function to draw a circle, a square, and a triangle.

## Let's Make: A Simple Pet Simulator

Let's use functions to make a program that simulates taking care of a pet!

```python
def feed_pet(pet_name):
    print(pet_name + " is eating. Yum!")

def play_with_pet(pet_name):
    print("You're playing with " + pet_name + ". So fun!")

def pet_sounds(pet_name, sound):
    print(pet_name + " says " + sound + "!")

# Let's use our pet simulator
pet_name = input("What's your pet's name? ")

feed_pet(pet_name)
play_with_pet(pet_name)
pet_sound = input("What sound does your pet make? ")
pet_sounds(pet_name, pet_sound)
```

Can you add a new function to make your pet go to sleep? What would it print?

## Great Job!
You've learned how to create and use functions in Python! Functions help us organize our code and make it easy to reuse. Keep practicing and have fun with your new Python skills!