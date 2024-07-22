# Day 4: Animated Scene Project

## Objective
Create a short animated scene with multiple sprites and interactions using Scratch 3.

## Step-by-Step Guide

1. Set Up the Project
   - Open [Scratch](https://scratch.mit.edu/projects/editor/) and start a new project.
   - Click "Choose a Backdrop" and select a suitable background for your scene.

2. Create Sprites
   - Click "Choose a Sprite" to add at least three different character sprites.
   - Position the sprites on the Stage using the mouse or by setting x and y coordinates in the Sprite Info pane.

3. Design Sprite Costumes
   - For each sprite:
     - Click the Costumes tab.
     - Click "Choose a Costume" or use the paint editor to create at least two additional costumes for different poses or expressions.
     - Rename costumes clearly (e.g., "happy", "sad", "walking") by clicking on the costume name.

4. Animate the Main Character
   - Select your main character sprite in the Sprite Pane.
   - Add these blocks:
     - "when green flag clicked" (from Events category)
     - "switch costume to [costume1 v]" (from Looks category)
     - "go to x: (-180) y: (-100)" (from Motion category)
     - "repeat (10)" (from Control category)
       - "switch costume to [walking1 v]"
       - "wait (0.2) seconds" (from Control category)
       - "switch costume to [walking2 v]"
       - "wait (0.2) seconds"
       - "change x by (20)" (from Motion category)

5. Add Character Dialogue
   - After the walking animation, add:
     - "switch costume to [happy v]" (from Looks category)
     - "say [Hello! Welcome to our animated scene!] for (3) seconds" (from Looks category)

6. Animate the Second Character
   - Click on your second character sprite in the Sprite Pane.
   - Add these blocks:
     - "when green flag clicked" (from Events category)
     - "wait (4) seconds" (from Control category)
     - "glide (2) secs to x: (0) y: (0)" (from Motion category)
     - "switch costume to [waving v]" (from Looks category)
     - "say [Hi there! Nice to see you!] for (3) seconds" (from Looks category)

7. Create Interactive Elements
   - Add a new sprite for an interactive object (e.g., a magical item or animal).
   - Add these blocks to the new sprite:
     - "when this sprite clicked" (from Events category)
     - "play sound [magic sound v]" (from Sound category)
     - "repeat (5)" (from Control category)
       - "change [color v] effect by (25)" (from Looks category)
       - "wait (0.1) seconds" (from Control category)
     - "broadcast [magic happens v]" (from Events category)

8. Respond to Interactions
   - Go back to your main character sprite.
   - Add a new script with these blocks:
     - "when I receive [magic happens v]" (from Events category)
     - "switch costume to [surprised v]" (from Looks category)
     - "say [Wow! Did you see that?] for (2) seconds" (from Looks category)

9. Add Background Animation
   - Click on the Stage in the bottom-left corner of the Sprite Pane.
   - In the Backdrops tab, add a second backdrop (e.g., a nighttime version of the scene).
   - In the Stage's Code tab, add:
     - "when green flag clicked" (from Events category)
     - "wait (10) seconds" (from Control category)
     - "switch backdrop to [backdrop2 v]" (from Looks category)

10. Final Character Interaction
    - Click on your third character sprite in the Sprite Pane.
    - Add this script:
      - "when backdrop switches to [backdrop2 v]" (from Events category)
      - "show" (from Looks category)
      - "glide (2) secs to x: (100) y: (0)" (from Motion category)
      - "say [What a magical evening!] for (3) seconds" (from Looks category)

11. Add Sound Effects and Music
    - For each sprite and the Stage:
      - Click the Sounds tab.
      - Click "Choose a Sound" to add appropriate sound effects or background music.
    - Incorporate these sounds into your scripts using "play sound [chosen sound v]" blocks (from Sound category).

12. Test and Refine
    - Click the green flag to start your animation.
    - Watch the entire scene and make sure all animations, dialogues, and interactions occur as intended.
    - Adjust timing, movements, and dialogue as needed for a smooth flow.

Remember to save your project regularly using "File" > "Save now" in the top menu.