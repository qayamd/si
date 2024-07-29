# Makey Makey Adventure: Catch the Apple Game

## What You Need
- Makey Makey kit
- Computer
- Internet
- Alligator clips
- Play-doh or aluminum foil

## Let's Make a Game!

### 1. Open Scratch (5 minutes)
1. Go to [Scratch](https://scratch.mit.edu/projects/editor/)
2. If you see a cat on the screen, you're ready to start!

### 2. Create Your Game (25 minutes)

#### Remove the Cat
1. Find the cat picture in the bottom right corner
2. Right-click on it
3. Click "delete"

#### Add a Basket
1. Click the blue button with a cat face at the bottom right
2. Type "basket" in the search box
3. Click on a basket you like

#### Add an Apple
1. Click the blue cat face button again
2. Type "apple" in the search box
3. Click on an apple you like

#### Make the Basket Move
1. Click on your basket in the bottom right corner
2. Find the yellow "Events" category on the left
3. Drag out "when green flag clicked"
4. Find the blue "Motion" category
5. Drag out "go to x: 0 y: 0" and snap it under the yellow block
6. Change the y number to -150
7. Find the orange "Control" category
8. Drag out "forever" and snap it under the blue block
9. Go back to "Control" and drag out two "if...then" blocks inside the "forever" block
10. Go to the light blue "Sensing" category
11. Drag out "key (space) pressed?" into the first "if" block
12. Click on "space" and change it to "left arrow"
13. Do the same for the second "if" block, but choose "right arrow"
14. Go back to "Motion" and drag "change x by 10" into both "if" blocks
15. Change the number to -10 for the left arrow block

#### Make the Apple Fall
1. Click on your apple in the bottom right corner
2. Drag out "when green flag clicked" from "Events"
3. Snap on a "forever" block from "Control"
4. From "Motion", add "go to x: 0 y: 0" inside the "forever"
5. Change the x to "pick random -240 to 240" (find this in the "Operators" category)
6. Change the y to 180
7. From "Control", add "repeat until" inside the "forever", under the "go to" block
8. From "Sensing", put "touching (mouse-pointer)" in the "repeat until" block
9. Change "mouse-pointer" to your basket's name
10. Inside the "repeat until", add "change y by -5" from "Motion"
11. After the "repeat until", add an "if...then" from "Control"
12. Put "touching (basket)" in the "if" part
13. Inside the "if", add "play sound (pop)" from "Sound"

#### Add a Score
1. Click "Variables" on the left
2. Click "Make a Variable"
3. Type "Score" and click OK
4. Drag "set Score to 0" into your apple's code, right after "when green flag clicked"
5. Add "change Score by 1" inside the "if...then" block at the end of your apple's code

### 3. Connect Makey Makey (10 minutes)
1. Plug your Makey Makey into the computer
2. Connect a clip to "Earth" on Makey Makey
3. Connect clips to "Left Arrow" and "Right Arrow"
4. Attach the other ends to play-doh or foil
5. Hold "Earth" and touch left and right to move the basket

### 4. Play Your Game!
- Click the green flag to start
- Catch as many apples as you can!

### 5. Make It Better
- Try adding more fruits
- Make the apple fall faster as you score more
- Add fun sounds or colors

Remember: If you get stuck, ask a friend or teacher for help. Have fun!
