# Learning Log Entry: **Selection Structure**

**a) What concept did you implement?**

The concept is *Selection Structure*, in which I used if and else statements for the bulk of my code.

*Examples are:* 

if (insidePlayArea && !collide(newX, newY)) {

  x = newX;
  
  y = newY;
  
  moved = true; 
  
} else {

  dir = int(random(4)); // Change to random direction if path is blocked
  
}

**b) Where did you use it, and why did you implement it that way?**

I used if-else statements in the cop movement function to handle the AI. The problem I had to solve was making sure the cops didn't just walk through walls or get stuck forever. The if statement checks if the next spot the cop wants to move to is empty. If it's a wall (the else part), the cop immediately picks a new random direction to walk in instead.

**c) What challenges did you encounter, and how did you fix them?**

A big issue was that the cops would sometimes vibrate against a wall. I realized it was because they weren't changing direction until they were already inside the wall. I fixed this by calculating their "next" position first and checking it before actually moving them.
