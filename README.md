
# N-Queens Visualizer

## Overview

The N-Queens Visualizer is a Java Swing application that visually demonstrates the process of solving the N-Queens problem using a backtracking algorithm. The goal of the N-Queens problem is to place N queens on an NxN chessboard such that no two queens can attack each other. This application allows users to visualize the placement of queens and the backtracking steps involved in finding a solution.

## Features

-   **Dynamic Board Size**: Users can specify the size of the chessboard (N) at runtime.
-   **Speed Control**: Users can control the speed of the visualization using a slider.
-   **Start/Stop Functionality**: Users can start and stop the visualization at any time.
-   **Multiple Solutions**: Users can view multiple solutions by clicking the "Next Solution" button.

## Requirements

-   Java Development Kit (JDK) 8 or later
-   Integrated Development Environment (IDE) such as IntelliJ IDEA, Eclipse, or NetBeans (optional but recommended)

## How to Run

1.  **Clone the Repository**: Download or clone the repository to your local machine.
2.  **Compile the Code**: Open a terminal or command prompt and navigate to the directory containing the source code. Compile the code using the following command:
    
    bash
    
    Copy code
    
    `javac NQueensVisualizer.java` 
    
3.  **Run the Application**: After compiling, run the application using the following command:
    
    bash
    
    Copy code
    
    `java NQueensVisualizer` 
    
4.  **Follow the Prompts**: Enter the size of the board (N) and the initial speed (in milliseconds) when prompted.

## Usage

-   **Start/Stop Button**: Click the "Start" button to begin the visualization. The button text will change to "Stop". Click "Stop" to pause the visualization.
-   **Next Solution Button**: After finding a solution, click the "Next Solution" button to clear the board and find the next solution.
-   **Speed Slider**: Adjust the speed of the visualization using the slider at the bottom of the window.

## Code Explanation

The main components of the application are:

1.  **NQueensVisualizer Class**: This class extends `JFrame` and contains the main logic and GUI components for the visualization.
2.  **getSizeFromUser() and getSpeedFromUser() Methods**: These methods prompt the user to enter the size of the board and the initial speed.
3.  **solvePuzzle() Method**: This method initiates the solving process and displays a success or error message.
4.  **findSolution() Method**: This method starts the backtracking algorithm.
5.  **clearBoard() Method**: This method clears the board for the next solution.
6.  **isSafe() Method**: This method checks if it's safe to place a queen at the given position.
7.  **solveNQueens() Method**: This method contains the backtracking logic to solve the N-Queens problem.
8.  **storeSolution() and isDuplicateSolution() Methods**: These methods handle the storage and checking of unique solutions.
9.  **updateGUI() Method**: This method updates the GUI to show the placement and removal of queens.
10.  **delay() Method**: This method introduces a delay to visualize the steps.

## Troubleshooting

-   **Invalid Input**: Ensure that the input for the board size and speed are valid integers.
-   **Performance**: Larger board sizes may result in longer computation times. Adjust the speed slider to manage the visualization speed.

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to improve the application.

## License

This project is licensed under the MIT License.
