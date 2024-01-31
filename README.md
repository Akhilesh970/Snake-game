# Snake-game
The snake Game project is composed in Python. The project file contains python script 
(snake.py). This is a simple GUI based method game which is developed using python’s 
package named pygame. In gameplay, it’s a single player game, where the player (Snake) has 
to eat all the fruits in order to grow snake longer. 
After starting the game, a GUI appears. Then the player has to control the snake. The main 
thing in this GUI based game is that the player just has to press “arrow keys” in the keyboard
to move the snake. At the top of the board, it displays a current player score. The player 
needs to catch the maximum number of fruits without hitting the wall or itself. All the game 
movements are to be performed manually by the player. While playing the game, make sure 
the snake should not cross the edges and should not snake touches its own tail in the game. 
Otherwise, player will die.
The game also consists of a high score module where the winner is assigned specific points 
based on the ranking and is stored in a database. The score is parsed from the variable to the 
SQL database.
The 2D GUI is designed using Pygame python. The gameplay design is simple and clean that 
the user won’t find it difficult to use and understand. For the gaming environment, the project 
uses various images to provide real-time experience.
# Description of Game:
The current snake game is a single player game. The game interface is built in 2D format.
The game is displayed in the pygame window. Here, it consists of two points where one is 
movable while the other is fixed. The movable point is the snake while that of the point at 
fixed location is the food. Whenever the snake gets the food the length of snake increases by 
one. The speed of the snake can be altered from the code. The player controls a long, thin 
creature, resembling a snake, which roams around on a bordered plane, picking up food (or 
some other item), trying to avoid hitting its own tail or the edges of the playing area. Each 
time the snake gets a piece of food, its tail grows longer by one, Also, the player score 
increases by one and making the game increasingly difficult. The user controls the direction 
of the snake's head (up, down, left, or right), and the snake's body follows.
A console window is created as soon as the game starts. The game will terminate if the snake 
head collides with any of the window's boundaries or with its own tail. Whenever the game is 
finished, the score is displayed in the centre of the window. The GUI is developed using 
pygame and various image files are used to create the interface. The interface is divided into 
various sections and each section lead up to different functionalities. The limitations with the 
existing system is that the game has no dedicated storage allocated to store the user’s 
information and performance statistics. The game has no information regarding the user so 
every time the game is executed it is like the game is running for the first time.
# Snake game logic:
In this snake game, if the player hits the boundaries of the screen, then he loses. To specify 
that, I have made use of an ‘if’ statement that defines the limits for the x and y coordinates of 
the snake to be less than or equal to that of the screen. Also, make a not over here that I have 
removed the hardcodes and used variables instead so that it becomes easy in case you want to 
make any changes to the game later on.
In pygame, we have this thing called Rect,.Rects make collision detection easy, You can also 
use Rect on images, any rectangular object works, It can also be circular. Now to make 
a Rect, we have to use Pygame.Rect() method We have to pass in the x coordinate as the 
first argument, y coordinate as the 2nd argument, and width and height as the 3rd and 4th 
argument respectively In our case, we first pass the snakes x coordinate, y coordinate, it's 
width and height Now rects have a lot of methods available, one is colliderect(), This 
method takes another Pygame.Rect() as argument and checks if they two collide with each 
other In our case, we pass fruit_pos transforming as Rect to the colliderect method. If this 
returned true, fruit_spawn will be true, so new fruits will be generated and the score will be 
increased.The game will terminate if the snake head collides with any of the window's 
boundaries or with its own tail
