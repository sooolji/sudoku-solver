# Sudoku-Solver
This is my first project for learning python. A sudoku solver using the backtracking algorithm. Run main.py to play sudoku.

# About Sudoku

Sudoku consists of filling a 9 x 9 cube of cells arranged in 9 subgroups of 3 x 3 cells, with numbers from 1 to 9, according to the restriction that the same number must not be repeated in the same row, column, or subgroup of 9.

A Sudoku has several cells with an initial value, so we must start solving the problem from this partial solution without modifying any of the initial cells.

# Pseudocode Implementation for Sudoku Solver

This pseudocode outlines the logic for solving a Sudoku puzzle using backtracking.

## Step 1: Initialize the Sudoku Board
Define the Sudoku board as a 2D array `board` with dimensions 9x9. Each cell contains numbers from 0 to 9, where 0 represents an empty square.


## Step 2: Find Empty Squares
Create a function `find_empty(bo)` that iterates through the board to locate an empty square (represented by 0). Return the coordinates of the first empty square found; otherwise, return `None`.


## Step 3: Validate Number Placement
Implement a function `valid(bo, num, pos)` to check if a number `num` can be placed at a given position `pos`. This involves checking the row, column, and 3x3 box for existing occurrences of the number.


## Step 4: Solve Sudoku Using Backtracking
Create a recursive function `solve(bo)` that uses backtracking to fill in the board. It finds an empty square using `find_empty`, then tries placing numbers from 1 to 9 at the current position. If a number is valid and leads to a solution, it recursively attempts to fill the rest of the board. If no number can be placed, it resets the current position and continues with the next number.

## Step 5: Print the Sudoku Board
Develop a function `print_board(bo)` to display the board. Include separators between rows and columns to clearly delineate the 3x3 boxes.

## Step 6: Execute the Program
Finally, execute the program by printing the original board, attempting to solve it, and displaying the solved board if successful.




# Resources used for this Projects

You can view the video tutorials i use to create this project here: https://www.youtube.com/watch?v=eqUwSA0xI-s&t=871s

You can learn more about Sudoku here:
https://en.wikipedia.org/wiki/Sudoku

You can learn more about solving Sudoku here:
https://en.wikipedia.org/wiki/Sudoku_solving_algorithms
