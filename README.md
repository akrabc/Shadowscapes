# Shadowscapes
## How to install and run the game:
Click on the link , and extract the zip folder and right click and click on open in terminal. Then type "python shadowscapes_main.py" to play.

https://github.com/akrabc/Shadowscapes/blob/main/ShadowScapes.zip
## About the game:
Theme: Sleeking through the silent shadows.
The main objective of the game is to protect the princess from the enemies. There are multiple levels in the game, the user has to fight multiple enemies across different levels to save the queen.
As the level increases the geme gets tougher as the enemies become difficult to defeat.The enemy has total two attaking moves kick and punch apart from the ability to move forward and jump.There are three types of enemies: FlameJet Thrower,Ork and Witch.The strongest of them all is the FlameJet Thrower which can launch fireballs and launch flame as it comes nearer to the player.In accordance with our theme we have given a special ability to the player that is, the player can escape into a shadow world to escape the enemy for a limited time period from which the player will automatically be brought back to the normal world from the shadow world.To escape into this shadow world the player must come in contact with one of the multiple shadows placed in the game,when in contact with the shadow the palyer has to press the DOWN arrow key in order to escape into the shadow world.The maps which signify different worlds keep automatically changing.There are total 5 worlds in the game and 3 difficulty levels.The player will be provided with a menu to choose the difficulty level the player wants. 
## Control
UP array key:  To jump
DOWN arrow key: To escape into the shadow world.
RIGHT arrow key: To move ahead in the game
x key:
k key: To kick
LEFT arrow key: To left move (Only available in the final level)
## Code construct:
In the while running loop we have deifned the moves of the player including moving and attacking moves.Since we knew the exact number of enemies we would have ,we have used the Varaible 'variable' to bring the different enemies onto the main game.The enemies have predefined set of moves, when the enemy is at a certain distance from the user the enemy, only moves but as the enemy comes at a particular distance the enemy starta attacking and the health of the player decreases.All the enemies have fixed health and it depends upon the user how fast the user defeats the enemy.
For checking whether the player should attack or simply move closer to the player we are checking whether the x coordinates of the enemy are in a certain range of the x coordinate of the player for this we have made use of the 'in range' of function of python and accordingly we are bliting the different sprite sheets of moving and attakcing respectivley.
We have created a list of the different sprite sheets and we are iterating over the lists using the 'index' using the clock.The enemies come only one after another i.e untill the player kills one enemy the other player wont come.To implement this we have used to variables namely 'variable' and 'chekcer'. Eack enemy in the game has a particular variable and the variable is only incremented when the previous enemy is defeated. The work of the variable 'checker' is that it is used to take the intial coordinates of the enemy,initialse enemy health and alive state of enemy, after this the checker becomes 0 untill the enemy dies and it's time for the next enemy to come at which the checker becomes 1 and then again 0, this process happens for each and every enemy.
To move the enemy to the left we are decremented the x coordinate of the enemy untill the enemy sufficiently close at which the enemy x coordinate stops decrementing and the player starts attacking.At this point the player health starts decreasing for this we are using if-else statement to check the range and decrease the player health while the enemy is attacking.  
Since in the gamestate 4 which is also the final stage of the game the player has extra moves hence we have defined the controls of the player again separatly only for the gamestate 4.
Every time any enemy comes at a certain distance from the player the health of the palyer decreases , the health of the player is continuoasly being displayed on the top of the screen so that the player can keep a track of the health, if the player health decreases to zero before the final enemy is defeated the game ends. 
There are four different worlds before the final battle with the strongest mage. Each world has its own obstacles, and one shadow can be found at one point in each world. Pressing the DOWN arrow allows the player to escape the enemy by sneaking into the shadow world.
In the first four worlds, the player is fixed at one point on the screen, and we move the backgrounds and the sprite sheets according to the keys pressed.
In the final world against the final mage, the player can move both ways, but the player has to risk extra damage from the enemy, if he tries to dodge.
After the player defeats the final mage and moves out of that map, he meets up with the princess, held hostage, and they set out back to their kingdom.
The open source images from web has been taken and then the class spritesheet.py breaks the png into individual images. Then we made a list of these broken images and iterated through each image in loop.
## Gameplay:
https://clipchamp.com/watch/NCCSu8vYbKr  

https://clipchamp.com/watch/kFIUASfSsMw
## Credits:
Developed by Areen Ramesh Patil,Krishna Sai and Ramya Parsania.
Special Thanks to Zense IIIT Bangalore.
