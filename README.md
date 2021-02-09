# 5607project1
The code was compiled on Windows OS.

Extra features I implemented:
1. Animation without user input. The square will automatically move to the right even without a user.
2. Visually feedback when the user pressed the keyboard. When the user pressed the "space", the cube will jump a little bit then fall (follow the Newton motion equation).

Some difficulty I met:
1. Make files. Since there is no direction about how to make file and compile in windows system. It takes me a while to set up the basic structure working.
2. Rotation with specific direction. When I want to implement the rotation functionality, I assume the user could change direction when rotating the square. I thought of a lot of ways on how to recognize the clockwise or counterclockwise. Finally, I reviewed the materials and found the optimal solution--cross product.
3. There was a sudden jump bug I met at the beginning of the project. Whenever I drag the square, the square will jump to the final position (not smooth). Later on, I found this was a bug related to the initialization.
4. Precision when testing. Since the scale function will only be activated when the user clicked the corner, which is a relatively small point to choose precisely. Even harder for me to test and debug. I found a way to solve this by measuring the distance from the corner. If the distance is smaller than a certain value, the function will be called. 
