# 8-puzzle game solver with A* algorithm
A random given 8-puzzle is solved by using A* algorithm. In the txt files, you can see the Tree that is created for possible scenarious and the chosen moves to solve the puzzle. An example solved puzzle is already given in the txt files.

## Running the code
You can simply write just "make" to run the program.
### Make commands:
- **make compile:** compile the program.
- **make clean:** Delete the .exe file.
- **make run:** run the program.
- **make:** Do all 3 above.

## Initial State.txt
You can view the initial state (a random 8-puzzle) of the game with current scores.

![Screenshot 2024-11-27 at 02 15 32](https://github.com/user-attachments/assets/a578ddd5-2ac3-466a-8226-e10cd0ae4c1c)

## Tree.txt
You can view the decision tree of the algorithm. The objective of the algorith is to minimize the h_score. The picture below shows the first 3 levels of the tree. First level shows the possible states right after the initial state. Since the `h_score` of the middle and the last state are the same, the algorithm will explore both of the states. Second level of the tree shows the children of the middle and the last state of the first level. Since the `h_score` of the child of the last element is lower, algorithm chooses that state and move on.

![Screenshot 2024-11-27 at 02 15 46](https://github.com/user-attachments/assets/a6120aaf-3a5b-4961-8e1e-8272ac219c9e)

## Moves.txt
You can view the chosen moves for each state of the puzzle. The picture below shows the final moves of the puzzle. When the `h_score` is equal to zero, the puzzle is solved.

![Screenshot 2024-11-27 at 02 16 06](https://github.com/user-attachments/assets/7a4d2f13-800b-4c92-8ded-86598ac8af5c)
