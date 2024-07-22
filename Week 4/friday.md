# Python Lesson 5: Let's Make an Adventure Game!

## Let's Get Started
We'll use the same website as before to write our Python code. [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

## What We'll Learn Today
Today, we're going to use everything we've learned this week to make a fun text adventure game! You'll learn how to:
1. Plan a bigger program
2. Use all the Python stuff we learned in one project
3. Make your own interactive story game

## The Adventure Game Project

In this game, the player will:
- Move through different places
- Pick up items
- Use items to solve puzzles
- Try to reach a goal (like finding treasure or escaping a maze)

## Planning Our Game

Let's break down our game into steps:

1. Set up the game:
   - Make a list of rooms or places
   - Make a list for the player's backpack (inventory)
   - Choose a starting room
   - Make a way to check if the game is over

2. Make the main game loop:
   - While the game isn't over:
     - Tell the player where they are
     - Ask the player what they want to do
     - Based on what they choose:
       - If they want to move:
         - Ask which direction
         - If they can go that way, change the room
         - If not, tell them they can't go that way
       - If they want to look around:
         - Describe the room
       - If they want to check their backpack:
         - Show what items they have
       - If they want to take an item:
         - If there's an item in the room, put it in their backpack
         - If not, tell them there's nothing to take
       - If they want to quit:
         - End the game
     - Check if they've reached the goal:
       - If yes, they win and the game ends

3. Add puzzles or challenges:
   - In some rooms, check if the player has a specific item
   - If they do, let them use it to solve a puzzle or overcome an obstacle

## Building the Game

Now, let's start building our game! Remember to use:
- `print()` to describe rooms and give messages to the player
- `input()` to get the player's choices
- Lists for rooms and the player's backpack
- A `while` loop for the main game
- `if-elif-else` statements to handle different player actions
- Variables to keep track of what's happening in the game

Start simple with just two or three rooms and one item, then make your game bigger once it's working.

## Cool Ideas to Try

1. Add more rooms to your game. Can you make a bigger world to explore?
2. Create more items and puzzles. Maybe the player needs to find a key to unlock a door?
3. Add a scoring system. How many points should players get for finding items or solving puzzles?
4. Make different endings based on what the player does or their score.

## You Did It!

Great job on bringing all the Python stuff we learned this week into one big project! You're using variables to remember game information, lists to keep track of rooms and items, a loop to keep the game going, and if-else statements to make decisions based on what the player does. You're becoming a real Python programmer!