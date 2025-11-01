PRODIGY_SD_04 - Suduko Solver

Sudoku Solver in Python

This project is a Python-based Sudoku solver that uses the backtracking algorithm to fill in a 9x9 grid. It takes an incomplete puzzle and attempts to solve it by recursively trying valid numbers in empty cells.

 Features
 
- Accepts a 9x9 grid with empty cells represented by 0
- Uses backtracking to find a valid solution
- Prints the grid before and after solving
- Displays the grid with clear formatting and 3x3 box separators

How It Works

1. print_grid(grid)
Prints the Sudoku grid in a readable format. Empty cells are shown as . and vertical/horizontal lines separate the 3x3 boxes.

2. find_empty(grid)
Scans the grid for the first empty cell (value 0) and returns its position as (row, col). If no empty cells are found, it returns None.

3. is_valid(grid, num, pos)
Checks whether placing a number num at position pos is valid:
- Ensures num is not already in the same row
- Ensures num is not already in the same column
- Ensures num is not already in the same 3x3 box

4. solve(grid)
This is the main recursive function:
- Finds the next empty cell
- Tries numbers from 1 to 9
- If a number is valid, places it and recursively attempts to solve the rest
- If stuck, backtracks by resetting the cell to 0 and tries the next number

 Sample Output

Unsolved Sudoku:

5 3 . | . 7 . | . . . 
6 . . | 1 9 5 | . . . 
. 9 8 | . . . | . 6 . 
---------------------
8 . . | . 6 . | . . 3 
4 . . | 8 . 3 | . . 1 
7 . . | . 2 . | . . 6 
---------------------
. 6 . | . . . | 2 8 . 
. . . | 4 1 9 | . . 5 
. . . | . 8 . | . 7 9 

Solved Sudoku:

5 3 4 | 6 7 8 | 9 1 2 
6 7 2 | 1 9 5 | 3 4 8 
1 9 8 | 3 4 2 | 5 6 7 
---------------------
8 5 9 | 7 6 1 | 4 2 3 
4 2 6 | 8 5 3 | 7 9 1 
7 1 3 | 9 2 4 | 8 5 6 
---------------------
9 6 1 | 5 3 7 | 2 8 4 
2 8 7 | 4 1 9 | 6 3 5 
3 4 5 | 2 8 6 | 1 7 9 



How to Run

- Save the code in a file, e.g., sudoku_solver.py
- Run it using Python 3:
python sudoku_solver.py



Concepts Used

- Backtracking algorithm
- Recursion
- 2D list traversal
- Input validation
- Modular function design
