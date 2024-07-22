# Day 3: Music Maker Project

## Objective
Create a simple music creation tool with different instruments using Scratch 3.

## Step-by-Step Guide

1. Set Up the Project
   - Open [Scratch](https://scratch.mit.edu/projects/editor/) and start a new project.
   - Click "Choose a Backdrop" and select a music-themed backdrop.

2. Create Instrument Sprites
   - Click "Choose a Sprite" to add at least four different instrument sprites.
   - Position the sprites across the Stage using the mouse or by setting x and y coordinates in the Sprite Info pane.

3. Add Sounds to Instruments
   - For each instrument sprite:
     - Click the Sounds tab.
     - Click "Choose a Sound" to add appropriate sounds for the instrument from the Sound Library.

4. Program the Piano
   - Add these blocks to the piano sprite:
     - "when this sprite clicked" (from Events category)
     - "play sound [piano note v]" (from Sound category)
   - Duplicate this script for each piano note, changing the sound in each copy.

5. Create a Drum Set
   - Add these blocks to the drum sprite:
     - "when this sprite clicked"
     - "play drum [Snare Drum v] for (0.25) beats" (from Music category)
   - Duplicate this script for different drum sounds, changing the drum type in each copy.

6. Program the Guitar
   - Add these blocks to the guitar sprite:
     - "when this sprite clicked"
     - "set instrument to [Electric Guitar v]" (from Music category)
     - "play sound [guitar strum v]"

7. Set Up the Flute
   - Add these blocks to the flute sprite:
     - "when this sprite clicked"
     - "set instrument to [Flute v]" (from Music category)
     - "play note (60) for (0.5) beats" (from Music category)

8. Create a Beat Sequencer
   - Click "Choose a Sprite" to add a new sprite for a beat button.
   - Add these blocks to the beat button:
     - "when green flag clicked"
     - "forever"
       - "play drum [Snare Drum v] for (0.25) beats"
       - "wait (1) seconds" (from Control category)
     - "when this sprite clicked"
     - "stop [this script v]" (from Control category)

9. Add Volume Control
   - Click "Make a Variable" to create a variable called "Volume" for all sprites.
   - Click "Choose a Sprite" to add a slider sprite.
   - Add these blocks to the slider sprite:
     - "when green flag clicked"
     - "forever"
       - "set [Volume v] to (mouse y)" (from Sensing category)
   - For each instrument sprite, add "set volume to (Volume) %" (from Sound category) before playing sounds.

10. Create Record and Playback
    - Click "Choose a Sprite" to add record and play button sprites.
    - Click "Make a List" to create a list called "Recorded Sounds" for all sprites.
    - Add blocks to the record button:
      - "when this sprite clicked"
      - "delete all of [Recorded Sounds v]" (from Variables category)
      - "broadcast [start recording v]" (from Events category)
    - Add blocks to each instrument sprite:
      - "when I receive [start recording v]" (from Events category)
      - "forever"
        - "if <<mouse down?> and <touching [mouse-pointer v]?>> then" (from Sensing category)
          - "add [instrument name] to [Recorded Sounds v]" (from Variables category)
          - "wait (0.5) seconds"
    - Add blocks to the play button:
      - "when this sprite clicked"
      - "broadcast [play recording v]"
    - Create a new sprite for playback and add:
      - "when I receive [play recording v]"
      - "repeat (length of [Recorded Sounds v])" (from Variables category)
        - "play sound (item (1) of [Recorded Sounds v])" (from Variables and Sound categories)
        - "delete (1) of [Recorded Sounds v]" (from Variables category)

11. Test and Refine
    - Click the green flag to start the project.
    - Test all features and adjust as needed.

12. Extensions (Optional)
    - Add graphic effects when instruments are played using blocks from the Looks category.
    - Create a loop feature for recorded sequences using the "repeat" block.
    - Implement a simple music visualizer using the "loudness" block from the Sensing category.

Remember to save your project regularly using "File" > "Save now" in the top menu.