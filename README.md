# project:Snake Game in Python

## Problem Statement
    This project implements a simple Snake game using Python's turtle module. 
    The game involves controlling a snake to eat food and grow longer, while 
    avoiding collisions with the game boundaries and its own body.

 ## Implemented Functionalities
    1.Snake Movement: The player controls the snake's direction using arrow keys.
    2.Food Generation: Food items are generated on the screen, increasing snake length upon consumption.
    3.Collision Detection: Detects collisions with screen boundaries and snake's body.
    4.Game Over: Ends the game when collisions occur, displaying snake's final length.

## Code Components
    The code can be divided into several components:
      1. Variables Initialization: Key variables like food, snake, and aim are set up to track
      the food's position, the snake's body segments, and its current movement direction.
    2.Functions: Essential functions include change(x, y) to update the movement direction,
    inside(head) to check if a position is within bounds, and move() to manage the snake's movement,
    collision detection, and display updates.
    3.Setup and Configuration: The screen setup is defined using setup(), the turtle cursor is hidden 
    with hideturtle(), and key input is enabled using listen(). Key bindings are established with onkey()
    to link arrow key presses to the change() function. Additionally, the animation speed is adjusted using tracer().
    4.Game Loop: The core loop is established by calling move() recursively with ontimer(). This loop controls
    the continuous motion of the snake, collision checks, food generation, and updates the display.
    5,Execution: The game starts running when the script is executed. The done() function halts the game loop
    when the game ends, either due to a collision or other conditions.

## Important Functions

### 1. move(): 
    This function handles the core logic of the game. It moves the snake's head in the current direction,
    checks for collisions with boundaries or itself, updates the snake's position and length, generates new
    food when the snake consumes it, and refreshes the display. The function is recursively called with ontimer()
    to maintain continuous movement and gameplay.

### 2. change(x, y):
    This function allows the player to change the snake's movement direction by updating the aim vector.
    It takes x and y values representing the change in horizontal and vertical directions, respectively.
    This function is linked to arrow key presses using onkey().

## Usage
    1.Run the script using a Python interpreter (Python 3.x recommended).
    2.The game window will appear, displaying a snake and food.
    3.Use arrow keys to control the snake's movement.
    4.Try to guide the snake to consume food and grow longer while avoiding collisions with the screen boundaries and itself.
    5.The game will end if the snake collides with the boundaries or itself.

### Enjoy playing the Snake game!
