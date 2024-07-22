# Day 5: Choose Your Own Adventure Game

## Objective
Design a text-based adventure game with multiple paths and outcomes using Scratch 3.

## Step-by-Step Guide

1. Set Up the Project
   - Open [Scratch](https://scratch.mit.edu/projects/editor/) and start a new project.
   - Choose a simple backdrop or create a title screen for your game.

2. Create Variables
   - Click "Make a Variable" in the Variables category.
   - Create these variables for all sprites:
     - "CurrentScene" (to track the player's progress)
     - "Inventory" (to store items the player collects)

3. Design the Main Character
   - Click "Choose a Sprite" to add a sprite representing the player's character.
   - Position it on the left side of the stage.

4. Set Up the Story Text
   - Create a new sprite and name it "StoryText".
   - In the Costumes tab, use the text tool to create a text box covering most of the right side of the stage.

5. Create Choice Buttons
   - Create two sprite buttons labeled "Choice1" and "Choice2".
   - Position them at the bottom of the stage.

6. Program the Game Start
   - On the Main Character sprite, add these blocks:
     - "when green flag clicked" (from Events category)
     - "set [CurrentScene v] to (1)" (from Variables category)
     - "set [Inventory v] to []" (from Variables category)
     - "broadcast [UpdateScene v]" (from Events category)

7. Update the Scene
   - On the StoryText sprite, add these blocks:
     - "when I receive [UpdateScene v]" (from Events category)
     - "switch costume to [TextBox v]" (from Looks category)
     - "if <(CurrentScene) = (1)> then" (from Control category)
       - "say [You find yourself at the entrance of a mysterious cave. Do you want to enter or explore the surrounding forest?]" (from Looks category)
     - "else if <(CurrentScene) = (2)> then"
       - "say [You enter the dark cave. You see a flickering light to your left and hear strange noises to your right. Which way do you go?]"
     - "else if <(CurrentScene) = (3)> then"
       - "say [You explore the forest and find a magical amulet. Do you want to wear it or leave it?]"
   - Continue adding more scenes and outcomes as needed.

8. Program Choice Buttons
   - On the Choice1 sprite, add these blocks:
     - "when green flag clicked" (from Events category)
     - "forever" (from Control category)
       - "if <(CurrentScene) = (1)> then" (from Control category)
         - "show" (from Looks category)
         - "say [Enter the cave]" (from Looks category)
       - "else if <(CurrentScene) = (2)> then"
         - "show"
         - "say [Go towards the light]"
       - "else if <(CurrentScene) = (3)> then"
         - "show"
         - "say [Wear the amulet]"
       - "else"
         - "hide" (from Looks category)

   - Add another script to Choice1:
     - "when this sprite clicked" (from Events category)
     - "if <(CurrentScene) = (1)> then" (from Control category)
       - "set [CurrentScene v] to (2)" (from Variables category)
     - "else if <(CurrentScene) = (2)> then"
       - "set [CurrentScene v] to (4)"
     - "else if <(CurrentScene) = (3)> then"
       - "add [magical amulet] to [Inventory v]" (from Variables category)
       - "set [CurrentScene v] to (6)"
     - "broadcast [UpdateScene v]" (from Events category)

   - Create similar scripts for the Choice2 sprite, with different outcomes.

9. Add Inventory Management
   - Create a new sprite called "InventoryDisplay".
   - Add this script:
     - "when green flag clicked" (from Events category)
     - "forever" (from Control category)
       - "say (join [Inventory: ] (Inventory))" (from Looks and Variables categories)

10. Create Multiple Endings
    - Add more scenes to the StoryText sprite's script.
    - Create different endings based on the player's choices and inventory.

11. Add Sound Effects
    - Click the Sounds tab for relevant sprites.
    - Click "Choose a Sound" to add sound effects for different actions.
    - Add "play sound [chosen sound v]" blocks (from Sound category) at appropriate points in your scripts.

12. Test and Refine
    - Click the green flag to start your game.
    - Play through your game multiple times, testing all paths.
    - Adjust text, timing, and game logic as needed.
    - Ensure all choices lead to satisfying conclusions.

Remember to save your project regularly using "File" > "Save now" in the top menu.

Extensions (if time allows):
- Add simple animations or costume changes to represent different scenes.
- Implement a scoring system based on choices made.
- Create more complex branching paths with additional variables.