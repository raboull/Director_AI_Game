# Director_AI_Game

Developed with Unreal Engine 4. 

This project was part of the CPSC 599.11 (AI in Games) course at the University of Calgary. The goal of the project was have students apply an AI technique learned in class to a small scale game using Unreal Engine 4. Our team chose to use the concept of an AI Director to dynamically adjust the intensity of the game based on a model of the player's current state.

## Description

The player will control Rob, the robot astronaut, as he navigates the hostile envoronment of the alien planet on which he crash landed. In this endless side-scroller platformer, the player must avoid oncoming meteorite-like enemies while continuously recharging their battery power (health) with the battery packs found throughout the platforms. While the player's health will never completely deplete, it is possible to enter a "power saving mode", greatly reducing the player's movement speed. 

As this is an “endless” game, the goal is for the player to have fun at their own pace. The player’s score is directly related to the total distance they have traveled in the right direction -- keep on trying for your new high score!

## Controls



## Director AI Overview
The Director AI is aware of certain parameters of the current game session. The Director AI then uses these parameters to adjust the platforming difficulty of the upcoming level chunk, the number of health packs on the level chunk, and the frequency of enemy spawns.
The following  three parameters are used to model the current game intensity, and determine the difficulty of the next level chunk:
1)  Time taken to travel across the previous level chunk (time intensity)
2)  Number of enemies that collided with the player in the previous level chunk (hit intensity)
3)  Amount of health the player has remaining (health intensity)

If the overall intensity is low, the game difficulty will increase as a result: more enemy spawns, fewer health spawns, or more difficult platforming. Alternatively, after a period of high intensity, the game difficulty may decrease to give the player a short break. The calculated intensity levels are displayed on-screen.




## Authors

Roman Abdoullaev\
Daniel Chang\
Liana Tomecek

## Assets and Acknowledgements
[Character, platforms, meteorite, level items, and background sprites](https://www.gameart2d.com/freebies.html)\
[Improved camera movement inspiration](https://drive.google.com/file/d/1-pvYL14P3f2tW88xg-Nhr-LfU99FTQb1/view)
