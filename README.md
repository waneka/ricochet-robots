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
- Once set in motion, a robot may not change course or stop. They must continue in a straight line until the hit an obstacle
- An obstacle may be any wall, the outside edge of the board, another robot, the center square, or any diagonal colored barrier
- When a robot hits a colored barrier
  - If the robot is the same color as the barrier, they move though it as if it wasn't there
  - if the robot is a different color than the barrier, they bounce of it on a right angle
- Any time the Robot begins movement from a stopped position, that counts as 1 "move"

### Programming challenges
