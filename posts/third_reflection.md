# Learning Log Entry **Variables & Data Tracking**

**a) What concept did you implement?**

The concept is *Variables*, in which I used different data types to store and track information in my game. 

*Examples are:* 
int score = 0;   -points from coins
int lives = 3;   -chances left
boolean gamePaused = false;   -pause on/off
String currentScreen = "intro";   -current screen
char[] maze;   -maze layout
int playerX, playerY;   -player position
int copSpeed = 3;   -cop speed

**b) Where did you use it, and why did you implement it that way?**

I will use these variables to track the game state, positions, and progress. Score and lives will change during coin collection and cop collisions. CurrentScreen will decide which screen to show. Maze (char[]) will hold the map layout. PlayerX/Y will move with arrow keys. CopSpeed will increase each level. I chose int for numbers, boolean for pause, String for screen names, and char[] for maze because they fit the data perfectly and keep the plan simple.

**c) What challenges did you encounter, and how did you fix them?**

I first thought about a separate list for coins, but it was too complicated. I decided to keep coins as '*' in the maze array. This change simplified everything, cut extra variables, and made planning easier.
