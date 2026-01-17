# Learning Log Entry: **Variables & Data Tracking**

**a) What concept did you implement?**

The concept is *Variables*, in which I used different data types to store and track information in my game. 

*Examples are:* 

int score = 0;

int lives = 3;

String screen = "Intro";

boolean upPressed = false;

**b) Where did you use it, and why did you implement it that way?**

I used different types of variables to keep track of everything happening in the game. Integers are used for numbers like the score and how many lives the player has left. I used a String called screen to act as a state controller, which lets the program know if it should be showing the menu, the actual game, or the game over screen. I also used booleans for the movement keys; this is better than just checking for a key press because it lets the player move diagonally by holding two keys at once.

**c) What challenges did you encounter, and how did you fix them?**

At first, the player moved really jittery because I put the movement code directly inside the keyPressed function. I fixed this by using the boolean variables to track if a key was being held down and then moving the actual movement math into the draw loop so it checks the frame.
