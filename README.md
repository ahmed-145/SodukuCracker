# 🧩 Sudoku Solver in C++

## 📌 Overview

This is a fully functional **Sudoku Solver** written in C++ using **recursive backtracking**. It accepts input manually or from a file, solves the puzzle by exploring all valid possibilities, and prints the completed grid.

> ✔ Demonstrates algorithmic thinking (backtracking, recursion)  
> ✔ Clean OOP design with `SudokuGrid` and `SudokuSolver` classes  
> ✔ Terminal-based UI with robust input handling  
> ✔ Tracks recursive depth for educational/statistical purposes

---

## 🧠 Core Concepts

- **Recursive Backtracking Algorithm**
- **Constraint Validation (rows, columns, 3×3 subgrids)**
- **2D Array Manipulation**
- **Basic Object-Oriented Programming**
- **Input Parsing from File / Console**

---

## 🚀 Getting Started

### 🔧 Requirements

- C++11 or later
- Windows OS (uses `<Windows.h>`)
- Command-line terminal

> ⚠ Linux/Mac users: replace `<Windows.h>` with platform-agnostic code if needed.

### 🛠 Compile & Run

g++ -o sudoku_solver sudoku_solver.cpp
./sudoku_solver


📥 Input Methods
1. Manual Input
You will be prompted to enter 81 values one by one (row by row). Use 0 for empty cells.

2. File Input
Prepare a .txt file in the same directory with:

Exactly 81 numbers

Space-separated

0 represents empty cells

Example:

python-repl
Copy
Edit
5 3 0 0 7 0 0 0 0
6 0 0 1 9 5 0 0 0
...
When prompted, enter the filename (e.g., puzzle.txt).

🖥 Sample Output
text
Copy
Edit
++=====================================++
|| 5  3     || 6     7     || 9     2  ||
++-----------++-----------++-----------++
...
QED. Your puzzle has been solved!

The singleCellSolve() function was recursively called 2547 times.
📂 File Structure
bash
Copy
Edit
📁 SudokuSolver/
├── sudoku_solver.cpp  # Source code
├── puzzle.txt         # (Optional) Sample input file
└── README.md
🧠 What You Learn
Backtracking algorithm internals

Clean class design in C++

Input validation

Grid formatting and console output tricks

Tracking algorithmic complexity (recursion count)

🏗️ Future Enhancements
Add GUI using SDL/SFML

Optimize constraint checking with hash sets or bitsets

Implement a puzzle generator

Add difficulty estimator

📜 License
MIT License — feel free to use, modify, or extend the project.

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you’d like to change.

Want me to generate the file and send it over, or include badges, screenshots, or GitHub Actions in this README?
