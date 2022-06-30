# Amazon Coding Challenge
### Bright Network Intenship, June 2022

In this challenge, you are going to implement Amazon’s pathfinding algorithm for Amazon’s self-driving delivery vehicles. The self-driving vehicle will need to create a path on a 2D-grid that contains a starting point (x,y), a delivery point (x,y) and a number of obstacles. Your vehicle can navigate to any of the adjacent squares (even diagonally), as long as the squares are inbound and do not contain an obstacle.

_Ideally, output to command line_

## Phase 1:
- Implement a 10x10 grid that contains a starting point on (0,0), the delivery point on (9,9) and the following obstacles on locations (9,7) (8,7) (6,7) (6,8)
- Your algorithm should calculate a valid path avoiding the obstacles and reaching the delivery point.
- Your solution should print the path in the format of [(x1,y1), (x2,y2), ...] and also the number of steps


## Phase 2:
- Add an additional 20 randomly placed obstacles and print their location using the format [(x1,y1), (x2,y2), ...]
- The obstacles shoul not overlap existing ones and should not be placed at the start and delivery points
- Your algorithm should calculate a valid path avoiding the obstacles and reaching the delivery point.
- Your solution should print the path in the format of [(x1,y1), (x2,y2), ...] and also the number of steps.


## Bonus:
- In the event that your vehicle is unable to reach its destinantion, your algorithm should print "Unable to reach delivery point" and identify which obstacles need to be removed in order for the vehicle to reach its destination.
- Your algorith should suggest the least amount of obstacles using the format [(x1,y1),(x2,y2)...] in order for your vehicle to reach its destination.


## Future Work
- While outside the scope of the design brief, I would like to visualise the pathfinding bot useing PyGame
- Similarly, using PyGame to create an interactive grid may allow users to solve real-world pathfinding problems using this bot.
