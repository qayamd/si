# Day 2: "Catch the Falling Objects" Game

## Objective
Create a game where the player moves a sprite to catch falling objects, keeping score and avoiding obstacles using Scratch 3.

## Step-by-Step Guide

1. Set Up the Project
   - Open [Scratch](https://scratch.mit.edu/projects/editor/) and start a new project.
   - Click "Choose a Backdrop" and select a sky backdrop from the Backdrop Library.

2. Create the Player's Sprite
   - Click "Choose a Sprite" and add a sprite for the player (e.g., a basket or bowl).
   - Rename the sprite to "Player" by clicking on the text box above the sprite in the Sprite Pane.

3. Program Player Movement
   - Add these blocks to the Player sprite:
     - "when green flag clicked" (from Events category)
     - "forever" (from Control category)
       - "if <key [left arrow v] pressed?> then" (from Control and Sensing categories)
         - "change x by (-10)" (from Motion category)
       - "if <key [right arrow v] pressed?> then"
         - "change x by (10)"
       - "if on edge, bounce" (from Motion category)

4. Create Falling Objects
   - Click "Choose a Sprite" to add a new sprite for the falling object.
   - Add these blocks to the falling object sprite:
     - "when green flag clicked"
     - "forever"
       - "go to x: (pick random (-240) to (240)) y: (180)" (from Motion category)
       - "glide (1) secs to x: (pick random (-240) to (240)) y: (-180)" (from Motion category)
       - "if <touching [Player v]?> then" (from Control and Sensing categories)
         - "hide" (from Looks category)
       - "show" (from Looks category)

5. Add Score
   - Click "Make a Variable" in the Variables category.
   - Create a variable called "Score" for all sprites.
   - Add these blocks to the Player sprite:
     - "when green flag clicked"
     - "set [Score v] to (0)" (from Variables category)
   - In the falling object's code, inside the "if touching Player" block, add:
     - "change [Score v] by (1)" (from Variables category)

6. Display Score
   - Add these blocks to the Player sprite:
     - "when green flag clicked"
     - "forever"
       - "say (Score)" (from Looks category)

7. Add an Obstacle
   - Click "Choose a Sprite" to create a new sprite for an obstacle.
   - Program it similar to the falling object, but add:
     - "if <touching [Player v]?> then"
       - "stop [all v]" (from Control category)

8. Add Sound Effects
   - Click the Sounds tab for the falling object sprite.
   - Click "Choose a Sound" to add a sound.
   - In the sprite's code, add "play sound [your chosen sound v]" (from Sound category) when the object is caught.

9. Create a Game Over Screen
   - Click "Choose a Backdrop" to add a new backdrop for the game over screen.
   - Add these blocks to the Player sprite:
     - "when [obstacle v] touches [Player v]" (from Events category)
     - "switch backdrop to [game over backdrop v]" (from Looks category)
     - "say (join [Game Over! Your score: ] (Score)) for (2) seconds" (from Looks category)

10. Test and Refine
    - Click the green flag to start the game.
    - Test all game elements and adjust as needed.

11. Extensions (Optional)
    - Add levels that increase in difficulty using variables and "if then" blocks.
    - Create different types of falling objects worth different points.
    - Add a timer using the "timer" block from the Sensing category.

Remember to save your project regularly using "File" > "Save now" in the top menu.