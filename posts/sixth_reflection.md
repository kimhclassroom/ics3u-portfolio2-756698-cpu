# Learning Log Entry: **Arrays & Data Structures**

**a) What concept did you implement?**

The concept is *Arrays & Data Structures*, for holding many values like the coins in my map.

*Examples are:* 

int[] coinX = new int[COIN_COUNT];

int[] coinY = new int[COIN_COUNT];

boolean[] taken = new boolean[COIN_COUNT];

**b) Where did you use it, and why did you implement it that way?**

I used three arrays to store all the coin data. Using arrays is the best way to handle multiple items because you can use a single index (like i) to find the X position, Y position, and whether it’s been collected for any specific coin. This makes the code much cleaner and makes it easy to add more coins later just by changing the COIN_COUNT variable.

**c) What challenges did you encounter, and how did you fix them?**

It was tricky making sure the coins didn't spawn on top of each other. I had to use a nested loop inside my coin setup function to check the distance between the new coin and all the old ones. If they were too close, I told the program to try a different random spot.


