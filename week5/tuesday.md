# Makey Makey Adventure: Turn the World into a Computer! 

[Day 1 content remains the same]

## Day 2: Create Your Own Makey Makey Game in Scratch

### What You'll Need
- Makey Makey kit
- Computer with internet access
- Alligator clips
- Conductive materials (aluminum foil, fruits, play-doh, etc.)

### Let's Make a Game!

Today, we're going to create a simple but fun game using Makey Makey and Scratch. We'll make a "Catch the Apple" game where you control a basket to catch falling apples.

#### 1. Set Up Scratch (5 minutes)
1. Go to [https://scratch.mit.edu/](https://scratch.mit.edu/)
2. Click on "Create" to start a new project
3. If you're not signed in, you can still create, but you won't be able to save your project online

#### 2. Create Your Game (25 minutes)

Follow these steps to create your game:

1. Delete the cat sprite by clicking the trash can icon next to it
2. Add a new sprite for the basket:
   - Click the "Choose a Sprite" button at the bottom right
   - Search for "basket" and select one you like

3. Add an apple sprite:
   - Click "Choose a Sprite" again
   - Search for "apple" and select one

4. Program the basket:
   - Click on the basket sprite
   - Add this code:
     ```scratch
     when green flag clicked
     go to x: (0) y: (-150)
     forever
       if <key (left arrow v) pressed?> then
         change x by (-10)
       end
       if <key (right arrow v) pressed?> then
         change x by (10)
       end
     ```

5. Program the apple:
   - Click on the apple sprite
   - Add this code:
     ```scratch
     when green flag clicked
     forever
       go to x: (pick random (-240) to (240)) y: (180)
       repeat until <touching (basket v)?>
         change y by (-5)
       end
       if <touching (basket v)?> then
         play sound (pop v)
       end
     ```

6. Add a score:
   - Click on the apple sprite
   - Add a variable called "Score":
     - Go to the Variables category
     - Click "Make a Variable"
     - Name it "Score" and click OK
   - Add this code to the apple sprite, right after the "if touching basket" block:
     ```scratch
     change [Score v] by (1)
     ```

7. Test your game:
   - Click the green flag to start
   - Use the left and right arrow keys to move the basket
   - Try to catch the falling apples!

#### 3. Connect Makey Makey (10 minutes)
Now, let's use Makey Makey to control our game:

1. Connect your Makey Makey to the computer
2. Connect one alligator clip to "Earth" on the Makey Makey
3. Connect two more clips to "Left Arrow" and "Right Arrow"
4. Connect the other ends of these clips to conductive objects (like fruits or aluminum foil)
5. Hold the "Earth" connection and touch the left and right objects to control your basket

#### 4. Extension Ideas (5 minutes)
Here are some ways you can make your game even better:

- Add more falling objects (like different fruits)
- Create levels that get faster as you score more points
- Add a "Game Over" screen if you miss too many apples
- Use different sounds for catching different objects
- Create a background that changes color based on your score

Remember:
- Be creative! There's no wrong way to improve your game.
- If something doesn't work, don't give up! Problem-solving is part of the fun.
- Ask your teacher for help if you get stuck.

Have fun playing and improving your Makey Makey-controlled Scratch game!