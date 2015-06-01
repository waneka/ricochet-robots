# Ricochet Robots
An attempt at programming a web-based multi-player version of the game Ricochet Robots
- The object of the game is to move the correctly colored robot to the correct tile on the game board in as few "moves" as possible

### Basic Rules
http://zmangames.com/rulebooks/Ricochet_Robots.pdf
- Players have a set time that they are able to search for the shortest route
- During the game time, players mentally search for the shortest route possible
- When a player finds an accurate route they enter the number of moves needed
- At the end of the time, the player that claims the shortest route must validate their solution
  - if the solution was successfully validated, that player receives a token
  - if not, the player with the next shortest route claim must validate their solution, and so on

### How Robots Move
- Once set in motion, a robot may not change course or stop. It must continue in a straight line until it hits an obstacle
- An obstacle may be any wall, the outside edge of the board, another robot, the center square, or any diagonal colored barrier
- When a robot hits a colored barrier
  - if the robot is the same color as the barrier, it moves though the square as if the barrier wasn't there
  - if the robot is a different color than the barrier, it will bounce off it in a right angle, continuing the move until it hits another barrier
- Any time the Robot begins movement from a stopped position, that counts as 1 "move"

### Programming Considerations
- What's the data shape?
- How will the robot "move" through the data?
- How will the robot move through the board, visually?
- What's the UI for each player validating their solution?
- Keeping score

### Extra Credit
- Websockets to connect multiple players
- Algo for shortest possible route to display after the winning player has collected their token