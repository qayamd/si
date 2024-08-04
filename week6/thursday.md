# Python Lesson 4: Fun with Lists

## Let's Get Started
Remember our coding playground? [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
After this lesson, you'll know how to:
1. Understand what lists are in Python
2. Create lists and access items in them
3. Change, add, and remove items in lists
4. Do cool operations with lists

## Part 1: What are Lists?

A list in Python is like a container that can hold lots of things. It's great when you want to keep similar things together. Think of it like a toy box where you can keep different toys!

## Part 2: Creating Lists

To make a list, we use square brackets `[]` and put things inside, separated by commas. Here's how it looks:

```python
fruits = ["apple", "banana", "orange"]
print(fruits)
```

This will show: ["apple", "banana", "orange"]

### Your Turn:
1. Make a list of your three favorite colors.
2. Create a list of five numbers.

## Part 3: Accessing Items in Lists

We can get things from a list by their position. In Python, we start counting from 0.

```python
fruits = ["apple", "banana", "orange"]
print(fruits[0])  # This will show "apple"
print(fruits[1])  # This will show "banana"
print(fruits[-1])  # This will show "orange" (counting from the end)
```

### Your Turn:
1. Make a list of five animals.
2. Print the first, third, and last animals from your list.

## Part 4: Changing Items in Lists

We can change items in a list by their position:

```python
fruits = ["apple", "banana", "orange"]
fruits[1] = "grape"
print(fruits)  # This will show ["apple", "grape", "orange"]
```

### Your Turn:
1. Make a list of three foods you like.
2. Change the second food to something different.

## Part 5: Adding and Removing Items

We can add things to a list using `append()` or `insert()`:

```python
fruits = ["apple", "banana"]
fruits.append("orange")  # Adds to the end
fruits.insert(1, "grape")  # Adds "grape" at position 1
print(fruits)  # Shows ["apple", "grape", "banana", "orange"]
```

We can remove things using `remove()` or `pop()`:

```python
fruits = ["apple", "banana", "orange"]
fruits.remove("banana")  # Removes "banana"
last_fruit = fruits.pop()  # Removes and returns the last item
print(fruits)  # Shows ["apple"]
print(last_fruit)  # Shows "orange"
```

### Your Turn:
1. Make a list of three hobbies.
2. Add a new hobby to the end.
3. Remove the second hobby.

## Part 6: Cool List Operations

We can do many cool things with lists:

```python
numbers = [1, 2, 3, 4, 5]
print(len(numbers))  # Shows how many items: 5
print(sum(numbers))  # Adds up all numbers: 15
print(max(numbers))  # Finds the biggest number: 5
print(min(numbers))  # Finds the smallest number: 1
print(sorted(numbers, reverse=True))  # Sorts in descending order: [5, 4, 3, 2, 1]
```

### Your Turn:
1. Make a list of five random numbers.
2. Find the length, sum, maximum, and minimum of your list.
3. Sort your list in descending order.

## Let's Make: Favorite Things Organizer

Let's make a program that helps organize your favorite things. Here's a framework to get you started:

```python
favorites = []

# TODO: Ask the user for their favorite things and add them to the list

# TODO: Print the list of favorite things

# TODO: Print how many favorite things are in the list

# TODO: Sort the list and print it again
```

Can you complete this program? Here's some pseudocode to help:

```
Repeat 3 times:
    Ask the user for a favorite thing
    Add it to the favorites list

Print the favorites list

Print the number of items in the favorites list

Sort the favorites list
Print the sorted list
```

Try running this program and then change it. Can you make it ask for a different number of favorite things?

## Great Job!
You've become a list master! You can now create, change, and do cool things with lists. In our next lesson, we'll use everything we've learned to make a fun adventure game!
