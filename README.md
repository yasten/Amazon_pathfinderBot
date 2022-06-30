# Amazon Coding Challenge
### Bright Network Intenship, June 2022

In this challenge, you are going to implement Amazon’s pathfinding algorithm for Amazon’s self-driving delivery vehicles. The self-driving vehicle will need to create a path on a 2D-grid that contains a starting point (x,y), a delivery point (x,y) and a number of obstacles. Your vehicle can navigate to any of the adjacent squares (even diagonally), as long as the squares are inbound and do not contain an obstacle.

_Ideally, output to command line_

## Phase 1:
- Implement a 10x10 grid that contains a starting point on (0,0), the delivery point on (9,9) and the following obstacles on locations (9,7) (8,7) (6,7) (6,8)
- Your algorithm should calculate a valid path avoiding the obstacles and reaching the delivery point.
- Your solution should print the path in the format of [(x1,y1), (x2,y2), ...] and also the number of steps


Output:
```
Number of steps:  10
Path:  [(0, 0), (1, 1), (2, 2), (3, 3), (4, 4), (5, 5), (6, 6), (7, 7), (8, 8), (9, 9)]
['0', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', 'X', 'X']
[' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', '*']
```

## Phase 2:
- Add an additional 20 randomly placed obstacles and print their location using the format [(x1,y1), (x2,y2), ...]
- The obstacles shoul not overlap existing ones and should not be placed at the start and delivery points
- Your algorithm should calculate a valid path avoiding the obstacles and reaching the delivery point.
- Your solution should print the path in the format of [(x1,y1), (x2,y2), ...] and also the number of steps.


Output:
```
Obstacle coordinates:  [(0, 7), (3, 3), (4, 3), (0, 0), (3, 2), (5, 9), (7, 4), (2, 2), (3, 4), (0, 1), (4, 5), (5, 3), (3, 0), (0, 6), (7, 2), (0, 3), (6, 2), (7, 3), (5, 5), (0, 2)]
Number of steps:  22
Path:  [(0, 0), (1, 1), (2, 1), (3, 1), (4, 1), (5, 1), (6, 1), (7, 1), (8, 2), (9, 3), (8, 3), (9, 4), (8, 4), (9, 5), (8, 5), (9, 6), (8, 6), (7, 6), (6, 6), (7, 7), (8, 8), (9, 9)]
['#', ' ', ' ', 'X', ' ', ' ', ' ', ' ', ' ', ' ']
['X', '#', '#', '#', '#', '#', '#', '#', ' ', ' ']
['X', ' ', 'X', 'X', ' ', ' ', 'X', 'X', '#', ' ']
['X', ' ', ' ', 'X', 'X', 'X', ' ', 'X', '#', '#']
[' ', ' ', ' ', 'X', ' ', ' ', ' ', 'X', '#', '#']
[' ', ' ', ' ', ' ', 'X', 'X', ' ', ' ', '#', '#']
['X', ' ', ' ', ' ', ' ', ' ', '#', '#', '#', '#']
['X', ' ', ' ', ' ', ' ', ' ', 'X', '#', 'X', 'X']
[' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', '#', ' ']
[' ', ' ', ' ', ' ', ' ', 'X', ' ', ' ', ' ', '#']
```

## Bonus:
- In the event that your vehicle is unable to reach its destinantion, your algorithm should print "Unable to reach delivery point" and identify which obstacles need to be removed in order for the vehicle to reach its destination.
- Your algorith should suggest the least amount of obstacles using the format [(x1,y1),(x2,y2)...] in order for your vehicle to reach its destination.


Output:
```
Obstacle coordinates:  [(7, 3), (1, 6), (1, 4), (3, 9), (0, 7), (5, 1), (2, 0), (2, 2), (6, 4), (8, 9), (7, 9), (4, 8), (0, 0), (9, 3), (6, 1), (4, 1), (1, 1), (3, 1), (7, 7), (3, 4)]
Unable to reach delivery point
['0', ' ', 'X', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', 'X', ' ', 'X', 'X', 'X', 'X', ' ', ' ', ' ']
[' ', ' ', 'X', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', 'X', ' ', 'X']
[' ', 'X', ' ', 'X', ' ', ' ', 'X', ' ', ' ', ' ']
[' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
[' ', 'X', ' ', ' ', ' ', ' ', ' ', ' ', ' ', ' ']
['X', ' ', ' ', ' ', ' ', ' ', 'X', 'X', 'X', 'X']
[' ', ' ', ' ', ' ', 'X', ' ', 'X', ' ', ' ', ' ']
[' ', ' ', ' ', 'X', ' ', ' ', ' ', 'X', 'X', '*']
```

## Future Work
- While outside the scope of the design brief, I would like to visualise the pathfinding bot useing PyGame
- Similarly, using PyGame to create an interactive grid may allow users to solve real-world pathfinding problems using this bot.
