# 🧩 C++ Sudoku Solver

A classic Sudoku puzzle solver implemented in C++. This application uses **recursive backtracking** to efficiently fill in incomplete Sudoku grids, either by user input or from a structured text file.

---

## 🔍 Features

- ✅ Manual puzzle input (via console)
- 📄 File-based puzzle input (text file with 81 space-separated values)
- 🧠 Backtracking algorithm for solving
- ✅ Validates each move with row, column, and 3x3 sub-grid checks
- 📊 Tracks recursion depth (calls to solver)
- 📈 Displays solved grid in a clean, formatted layout

---

## 📁 Input Format (for file-based input)

- Text file located in the same directory as the executable
- File name must be **≤ 20 characters**
- Must contain exactly **81 integers** (0–9) separated by spaces
  - Use `0` for empty cells
  - Example:
    ```
    5 3 0 0 7 0 0 0 0
    6 0 0 1 9 5 0 0 0
    ...
    ```

---

## 🛠 How to Compile

Make sure you're on **Linux**, **macOS**, or **MinGW** (no `Windows.h` dependency).

```bash
g++ -o SudokuSolver main.cpp
./SudokuSolver

📷 Sample Run

======================
    Sudoku Solver
======================

Welcome to Sudoku Solver!
    1. Input the puzzle by entering the values manually. (Enter 1)
    2. Input the puzzle by reading a file with values in it. (Enter 2)
    --> 2

Enter the name of the file that contains the Sudoku Puzzle.
    --> input.txt

++=====================================++
|| 5  3       || 6        || 9  8      ||
++-----------++-----------++-----------++
...

QED. Your puzzle has been solved!

The singleCellSolve() function was recursively called 5531 times.
🚀 Algorithm Used
The core logic is built on:

Backtracking to try potential values recursively

Constraint checking on:

Rows

Columns

3x3 sub-grids

🧪 Future Improvements
Add GUI using SFML or Qt

Difficulty rating for puzzles

Sudoku generator

Optimize with constraint propagation (e.g., dancing links / AC-3)
