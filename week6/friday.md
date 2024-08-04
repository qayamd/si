# Python Lesson 5: Let's Make an Adventure Game!

## Let's Get Started
Remember our coding playground? [Click here to open it](https://www.programiz.com/python-programming/online-compiler/)

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
     - Respond to the player's choice
   - Check if they've reached the goal

3. Add puzzles or challenges

## Building Your Adventure Game

Now it's your turn to build the game! Here's a framework to get you started, along with pseudocode for the main parts you need to implement:

```python
# Game setup
rooms = ["forest", "cave", "river", "mountain"]
inventory = []
current_room = "forest"
game_over = False
items = {"forest": "map", "cave": "torch", "river": "boat"}

# Main game loop
while not game_over:
    # 1. Print current location

    # 2. Get player's action

    # 3. Handle player's action
    if action == "move":
        # Handle movement
        pass
    elif action == "look":
        # Handle looking around
        pass
    elif action == "take":
        # Handle taking items
        pass
    elif action == "inventory":
        # Handle showing inventory
        pass
    elif action == "quit":
        # Handle quitting the game
        pass
    else:
        # Handle unknown command

    # 4. Check if player has won
```

Now, let's break down each part with pseudocode:

1. Printing current location:
   ```
   Print a message telling the player where they are
   ```

2. Getting player's action:
   ```
   Use input() to ask the player what they want to do
   Store the result in a variable called 'action'
   ```

3. Handling player's action:
   For "move":
   ```
   Ask the player where they want to go
   If the new room is in the list of rooms:
       Update current_room
       Print a message about moving
   Else:
       Print a message saying they can't go there
   ```

   For "look":
   ```
   Print a description of the current room
   If there's an item in the room:
       Print a message about seeing the item
   ```

  For "take":
   ```
   If there's an item in the current room:
       Add the item to the inventory
       Remove the item from the room
       Print a message about taking the item
   Else:
       Print a message saying there's nothing to take
   ```

   For "inventory":
   ```
   If the inventory is not empty:
       Print the contents of the inventory
   Else:
       Print a message saying the inventory is empty
   ```

   For "quit":
   ```
   Set game_over to True
   Print a goodbye message
   ```

4. Checking if player has won:
   ```
   If the current_room is "mountain" and "map" is in the inventory:
       Print a congratulations message
       Set game_over to True
   ```

Remember to use the comparison operators we learned:
- `==` to check if two things are equal
- `in` to check if something is in a list or dictionary
- `not in` to check if something is not in a list or dictionary

Try implementing each part of the game. If you get stuck, don't hesitate to ask for help!

## Cool Ideas to Try

Once you have the basic game working, here are some ideas to make it even better:

1. Add more rooms to your game. Can you make a bigger world to explore?
2. Create more items and puzzles. Maybe the player needs to find a key to unlock a door?
3. Add a scoring system. How many points should players get for finding items or solving puzzles?
4. Make different endings based on what the player does or their score.

## You're Doing Great!

Remember, building a game like this takes time and practice. Don't worry if you don't get everything perfect the first time. The important thing is that you're learning and having fun! Keep experimenting and improving your game.

Here are some tips to help you as you build your game:

1. Start small: Get the basic movement and looking around working first.
2. Test often: After you add each new feature, run your game to make sure it works.
3. Use print statements: If something isn't working, use print() to check the values of your variables.
4. Be creative: This is your game! Feel free to change the rooms, items, or add your own features.

## Wrapping Up

Congratulations on completing this Python course! Let's recap what you've learned:

- You started with basic print statements and variables
- You learned about if-else statements to make decisions
- You mastered loops to repeat actions
- You explored lists to store and manage collections of data
- And now, you've brought it all together to create your very own text adventure game!

You've come a long way in just a week. You're well on your way to becoming a Python programmer! Remember, the key to getting better at programming is practice. Keep coding, keep experimenting, and most importantly, keep having fun with it!

What will you create next?
