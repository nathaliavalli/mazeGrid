Overview

The MazeGridPanel class is a JPanel implementation for displaying and solving maze grids.
It provides methods to generate a maze, solve the maze, and visualize the maze using colors.

Features

Generates maze grids with specified rows and columns.
Solves the maze using an algorithm implemented in the solveMaze method.
Provides visualization of maze cells using different colors.
Implements maze generation and solving logic.


Usage

Instantiate the MazeGridPanel class with the desired number of rows and columns.
MazeGridPanel mazePanel = new MazeGridPanel(10, 10); // Example with 10 rows and 10 columns

Add the MazeGridPanel instance to a JFrame or another container.
JFrame frame = new JFrame("Maze Solver");
frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
frame.getContentPane().add(mazePanel);
frame.pack();
frame.setVisible(true);

The maze is generated and solved automatically upon instantiation.
Methods

generateMaze(): Generates a maze grid with walls and paths.
solveMaze(): Solves the generated maze using an algorithm implemented within the method.
generateMazeByDFS(): Extra credit method for generating a maze using Depth-First Search (DFS) algorithm.
visited(int row, int col): Checks if a cell has been visited during maze solving.


Implementation Details

The maze is represented as a grid of cells, with each cell containing information about its walls and neighbors.
Maze generation is implemented to create a random maze with paths and walls.
Maze solving is implemented using a stack-based algorithm to traverse the maze and find the solution.
