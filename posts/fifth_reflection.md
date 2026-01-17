# Learning Log Entry: **Repetition Structure**

**a) What concept did you implement?**

The concept is *Repetition Structure*, for loops and while loops to commence specific commands over and over.

*Examples are:* 

for (int i = 0; i < COIN_COUNT; i++) {

  if (!taken[i]) {
  
    image(coin, coinX[i], coinY[i], 40, 40);
    
  }
  
}

**b) Where did you use it, and why did you implement it that way?**

I used a for loop to handle the coins. Since there are 30 coins, it would be a huge waste of time to write 30 different lines of code to draw them. The loop starts at 0 and goes up to 29, checking each coin in the array. If the coin hasn't been "taken" yet, it draws the image on the screen.

**c) What challenges did you encounter, and how did you fix them?**

The loop worked, but it kept drawing the coins even after I collected them. I had to add the if (!taken[i]) check inside the loop so that the program knows to stop drawing that specific coin once the player touches it.

