# Snake-Game-Using-Python
reated a snake game using a python module named  “Pygame”. Basically, in this game, the user will control the movement of the snake through the keyboard arrows and direct the snake in the direction of food, as the snake eats the food the size of the snake will get increase...
Installation:
To work with this project you need to install pygame module via pip installation.

To install the module open your terminal and run the command below:

$ python -m pip install pygame

Explanation:
First, we will import the “pygame” module using the import keyboard. If it’s not there in your system then follow the particular command “pip install pygame” in your cmd. After importing the next step is to initialize the pygame with the .init() method, this is the most important step to execute.

→For a game, the basic need is to create a game window and this is the next step to be followed in this project with the help of “display.set_mode((width, height))” [In this, the parameters describe the size of the window]. With the help of “.fill(color)” we will fill the specific color in our window.

→ To make it attentive, we have set the title and icon with the help of “display.set_caption()” and “display.set_icon()” respectively for the game window.

→ Now, we have set the frames per second to be shown with the help of “pygame.time.Clock()”  which is available in the “time” module in python

→ We have initialized the two variables i.e. snake_block and snake_speed. Since to add any text we will need a font type and its size and that will be our next step via “pygame. font.SysFont(“Font name”,” size”)”, this function is provided by the “Sys” module

→ Now onwards, every step of this program is a part of our game and so to execute it will need a loop, and in game development, the theory works like that. So we will need a game loop and each step is known as an “event” under this, so we will execute each event under this game loop

→ For this loop, will make use of a while loop in which with the help of “pygame.event.get()”, we will run a for loop to see the events running. With the help of the “if condition” we will check the type of event by “.type()” and then we will execute the statements according to our need

→ Firstly, we have checked whether the event type is quit or not, if it is then close the window with the help of the “running” variable by making it false

→ Now the main element of this particular game is a snake and for this game, a rectangle will be considered as a part of the snake and for drawing so will make use of “pygame.draw.rect(surface, color,[left, top, width, height])”, in which surface is the game window and color will be in the format of RGB (red, green, blue)

→ The next most important step is to move the snake and for doing so we will use the “KEYDOWN” event, that is whenever the user will press down the keyboard arrows then due to that the snake will follow a particular direction and for doing so we have checked the event type under the if condition as “pygame. KEYDOWN”, and under that, we have checked the directions with the help of “K_LEFT”, “K_RIGHT”, “K_UP”, “K_DOWN”.If we will see correctly then this movement’s basic logic is to increase and decrease the values of x and y coordinates according to the directions

→ To keep all of this information in an updated way for our game window we have used “pygame. the display.update()”. This method will make sure to add up every process change.

→ In the next step, we have to set the boundaries of our game and by if condition we are doing so, we will just provide our ending coordinates as the conditions and give the event loop the command to over the game

→ The next step is to draw the food and we are again considering a rectangle as the food and will follow the same process as before. Now the logic is if the snake eats the food then the length of the snake should increase and the food should appear randomly at another location. For doing so, first of all, we will check the coordinates of the snake and food if they are equal then the food will again appear randomly at any position, and with the help of the “randrange” function in the “random” module and also will increase the length of snake by 1

→ The final step is to declare the score and for that, we have defined a function in which firstly we will render the value by “.render()”. Then we will draw it on the screen by the “.blit(value, color)” method.

This is how this pygame-based project works!!
