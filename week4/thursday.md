# Python Lesson 4: Fun with Lists

## Let's Get Started
We'll use the same website as before to write our Python code. [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what lists are in Python
2. Make lists and get things from them
3. Do cool stuff with lists

## Part 1: What are Lists?

A list in Python is like a container that can hold lots of things. It's great when you want to keep similar things together.

## Part 2: Making Lists

To make a list, we use square brackets `[]` and put things inside, separated by commas. Here's how it looks:

```python
fruits = ["apple", "banana", "orange"]
print(fruits)
```

This will show: ["apple", "banana", "orange"]

### Your Turn:
1. Make a list of your three favorite colors.
2. Show your list of colors.

## Part 3: Getting Things from Lists

We can get things from a list by their position. In Python, we start counting from 0.

```python
fruits = ["apple", "banana", "orange"]
print(fruits[0])  # This will show "apple"
print(fruits[1])  # This will show "banana"
```

### Your Turn:
1. Make a list of five animals.
2. Show the first and third animals from your list.

## Part 4: Cool List Tricks

We can add things to a list using `append()`:

```python
fruits = ["apple", "banana"]
fruits.append("orange")
print(fruits)  # This will show ["apple", "banana", "orange"]
```

We can also count how many things are in a list using `len()`:

```python
fruits = ["apple", "banana", "orange"]
print(len(fruits))  # This will show 3
```

### Your Turn:
1. Make a list of two foods you like.
2. Use `append()` to add another food to your list.
3. Show your list and then show how many foods are in it.

## Let's Make: Favorite Things Organizer

Let's make a program that helps organize your favorite things:

1. Start with an empty list called `favorites`.
2. Ask the user to tell you three of their favorite things.
3. Add each favorite thing to the list.
4. Show the list of favorite things.
5. Tell how many favorite things are in the list.

Here's how to start:

```python
favorites = []

for i in range(3):
    item = input("Tell me one of your favorite things: ")
    favorites.append(item)

print("Your favorite things are:", favorites)
print("You have", len(favorites), "favorite things in your list.")
```

Try running this program and then change it. Can you make it ask for a different number of favorite things?

## Great Job!
You've finished your fourth Python lesson! You learned how to make lists, get things from lists, and do cool stuff with lists. In our next lesson, we'll use everything we've learned to make a fun adventure game!