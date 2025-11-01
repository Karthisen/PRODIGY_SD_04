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
