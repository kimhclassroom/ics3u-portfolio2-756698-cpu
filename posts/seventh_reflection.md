# Learning Log Entry: **Custom Functions & Error Checking**

**a) What concept did you implement?**

The concept is *Custom Functions & Error Checking*, for making my own functions to help with the logic of the game and what and what should't happen.

*Examples are:* 

boolean overlap(int x1, int y1, int wx, int wy, int ww, int wh) {

  int x2 = x1 + 50;
  
  int y2 = y1 + 50;
  
  return !(x2 <= wx || x1 >= wx + ww || y2 <= wy || y1 >= wy + wh);
  
}

**b) Where did you use it, and why did you implement it that way?**

I wrote a custom function called overlap to handle all the hit detection in the game. It takes the coordinates of two objects and does the math to see if they are touching. This supports the game because I can use this one function for everything: checking if the player hits a wall, if they pick up a coin, or if they get caught by a cop.

**c) What challenges did you encounter, and how did you fix them?**

The biggest "error checking" I added was for spawning. I didn't want the player to start the game already inside a wall or on top of a cop. I used my overlap function inside a while loop when the level starts to keep re-rolling the player's spawn point until it finds a spot that is actually safe to stand in.
