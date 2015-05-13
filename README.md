Below you will find an explanation of the game play mechanics used in Daniel.  I hope this helps explain a few things and will reduce some of the learning curve.  In general, I attempted to make use of parent objects when I could so that adding additional items, characters, or enemies would be easier to maintain and implement successfully. This game was prepared for a class and was rushed, if you would like to make edits, there's a gamemaker file that you can use in the Daniel folder. The program was prepared with Gamemaker 8 for windows. 

How to play:
Use SPACE to use sword and attack enemies. Use keypad to move around. 

Battle:
During battle, if an enemy's health is not depleted completely they will be pushed back.  If they are destroyed, a small animation and sound is played upon their death.  If they hit Helena, her hit points are reduced by the amount specified by the enemy.  Helena is also pushed back and becomes invincible for a short period of time.  If all of her health is depleted, she loses one life.  If all of her lives are depleted the game ends, Helena turns into a ghost, and the game will restart.

Because the amount of health taken from Helena can be configured by enemy, I have added a script in the obj_helena object that detects a collision with obj_enemy_parent.  When you create an enemy, you need to put a new entry in this code for the enemy or Helena will not have any of her health taken away.

For obj_malgru, he has some artificial intelligence programmed into him.  Basically, this enemy will follow Helena when she gets close enough.  It is also smart enough to not "see" Helena when she is hidden behind walls.  Feel free to use this logic for any of your enemies if you want them following Helena.  

Final room:
The final room has a series of switches that must be clicked in the right order.  To click a switch, use the spacebar to hit it with your sword.  I will work on creating a text box that gives a clue on what to do in this room.

