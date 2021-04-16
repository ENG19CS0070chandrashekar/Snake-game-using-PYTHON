	ABSTRACT:
This simple Snake Game project is written in Python. The project file contains image files and python scripts (game.py, duplicate.py). GUI uses pygame library. Talking about the gameplay, it’s a single player game, where the player (Snake) has to eat all the apples in order to grow longer. The main objective of this game is to gain the highest score. While playing the game, make sure the snake should not cross the edges otherwise you’ll die.

A simple and clean GUI is provided for easy gameplay. The gameplay design is so simple that the user won’t find it difficult to use and understand. Different images are used in the development of this game project.
The thing you will need to do in order to develop the game using pygame is to install it on your system,to do that you can use the command which is given in below,

Pip pygame install:
And import the pygame module in system ,Once it is done,you can start with game development.


	OBJECTIVES OF THE PROJECT:
In this miniproject we will learn how to build the  snake game. The game is an arcade game and it has very simple logic, which is why it is an ideal example to demonstrate how to build games with Pygame.

The player is represented as snake, which grows if it eats an apple. The goal of the game is to eat as many apples as possible without colliding into yourself. This is very easy in the early phase of the game but is increasingly more difficult as the length of the snake grows.

Game logic:
The snake game has some rules:
o	If the snake eats an apple, the apple moves to a new position.
o	If the snake eats an apple, the snakes length grows.
o	If a snake collapses with itself or crosses the boundary, game over.

	REQUIREMENTS:
•	Hardware requirements:
           1.Secondary memory to store all the images and database.
           2.PC or laptop
•	Software requirements:
	
          1)Pycharm professional/Community latest version.
          2)Python 3.5 or more.
          3)Windows 8 or higher.
          4)Latest versions of all libraries.
          5)PYGAME module    
                                                                 
	Methodology :
       Steps to build snake game using python:
	Step-1. Installing Pygame
	Step-2. Create the Screen
	Step-3. Create the Snake
	Step-4. Moving the Snake
	Step-5. Game Over when Snake hits the boundaries
	Step-6. Adding the Food
	Step-7. Increasing the Length of the Snake
	Step-8. Displaying the Score 

	Step-1. Installing Pygame:
The first thing we will need to do in order to create games using Pygame is to install it on your systems. To do that, you can simply use the following command:
pip install pygame
Once that is done, just import Pygame and start off with your game development. 

	Step-2. Create the Screen:
To create the screen using Pygame, we will need to make use of the display.set_mode() function. Also, you will have to make use of the init()  and the quit() methods to initialize and uninitialize everything at the start and the end of the code. The update() method is used to update any changes made to the screen. There is another method i.e flip() that works similarly to the update() function. The difference is that the update() method updates only the changes that are made (however, if no parameters are passed, updates the complete screen) but the flip() method redoes the complete screen again.
CODE:
import pygame
pygame.init()
dis=pygame.display.set_mode((400,300))
pygame.display.update()
pygame.quit()
quit()

But when we run this code, the screen will appear, but it will immediately close as well. To fix that, you should make use of a game loop using the while loop before I actually

	Step-3. Create the Snake:
To create the snake, I will first initialize a few color variables in order to color the snake, food, screen, etc. The color scheme used in Pygame is RGB i.e “Red Green Blue”. In case you set all these to 0’s, the color will be black and all 255’s will be white. So our snake will actually be a rectangle. To draw rectangles in Pygame, you can make use of a function called draw.rect() which will help yo draw the rectangle with the desired color and size. 

	Step-4. Moving the Snake:
To move the snake, you will need to use the key events present in the KEYDOWN class of Pygame. The events that are used over here are, K_UP, K_DOWN, K_LEFT, and K_RIGHT to make the snake move up, down, left and right respectively. Also, the display screen is changed from the default black to white using the fill() method.
I have created new variables x1_change and y1_change in order to hold the updating values of the x and y coordinates.

	Step-5. Game Over when Snake hits the boundaries:
In this snake game, if the player hits the boundaries of the screen, then he loses. To specify that, I have made use of an ‘if’ statement that defines the limits for the x and y coordinates of the snake to be less than or equal to that of the screen. Also, make a not over here that I have removed the hardcodes and used variables instead so that it becomes easy in case you want to make any changes to the game later on.

	Step-6. Adding the Food:

Here, I will be adding some food for the snake and when the snake crosses over that food, I will have a message saying “Yummy!!”. Also, I will be making a small change wherein I will include the options to quit the game or to play again when the player loses.

	Step-7. Increasing the Length of the Snake:
The following code will increase the size of our sake when it eats the food. Also, if the snake collides with his own body, the game is over and you ill see a message as “You Lost! Press Q-Quit or C-Play Again“. The length of the snake is basically contained in a list and the initial size that is specified in the following code is one block.


	Step-8. Displaying the Score:

Last but definitely not the least, you will need to display the score of the player. To do this, I have created a new function as “Your_score”. This function will display the length of the snake subtracted by 1 because that is the initial size of the snake.

	Conclusion and future scope:


In the conclusion of this project, I would like to say that Python is a fun and easy programming language and while creating a project like this, it has not just been a good experience but it also helped in the development of my creativity and logical thinking. I would be more than happy to work on other projects in Python because it’s just amazing to work with Python. Also we have gained knowledge about the pygame module in python for the creation of games and after this project, we have the basic knowledge in the creation of games in python. This code is not yet completed. It can still be enhanced with additional features such as including background, graphics,& adding images,music ....etc











