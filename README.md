# N-Queens Problem 👑

A comprehensive Python implementation of the classic N-Queens Problem using recursion and backtracking algorithms, accompanied by detailed lecture materials.

## 📋 Table of Contents

- [Overview](#overview)
- [Problem Description](#problem-description)
- [Repository Contents](#repository-contents)
- [Features](#features)
- [Algorithm Approach](#algorithm-approach)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Complexity Analysis](#complexity-analysis)
- [Example Output](#example-output)
- [Learning Resources](#learning-resources)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)

## 🔍 Overview

The N-Queens Problem is a classic combinatorial problem in computer science and mathematics. This repository provides a complete solution implementation in Python along with comprehensive educational materials to help understand the backtracking approach.

## 🎯 Problem Description

The N-Queens Problem challenges us to place N chess queens on an N×N chessboard such that no two queens threaten each other. This means:

- No two queens share the same **row**
- No two queens share the same **column**
- No two queens share the same **diagonal** (both positive and negative diagonals)

For example, on a standard 8×8 chessboard, there are 92 distinct solutions to place 8 queens safely.

## 📁 Repository Contents

```
75-N-Queens-Problem/
│
├── N-Queens - Lecture.pdf    # Comprehensive lecture notes explaining the problem
│                              # and solution approach
│
└── N-Queens Problem.py        # Python implementation using backtracking
```

### 1. **N-Queens - Lecture.pdf**
   - Detailed explanation of the N-Queens problem
   - Step-by-step logic breakdown
   - Board representation techniques
   - Safety check mechanisms
   - Complexity analysis
   - Code walkthrough

### 2. **N-Queens Problem.py**
   - Clean, well-documented Python implementation
   - Recursive backtracking algorithm
   - Efficient queen placement and validation
   - Solution visualization

## ✨ Features

- ✅ **Recursive Backtracking**: Efficient algorithm that explores all possible configurations
- ✅ **Safety Validation**: Comprehensive checks for row, column, and diagonal conflicts
- ✅ **Scalable Solution**: Works for any board size N
- ✅ **Educational Materials**: Includes detailed lecture PDF for learning
- ✅ **Clean Code**: Well-structured and documented Python implementation
- ✅ **Multiple Solutions**: Can find all possible solutions for a given N

## 🧩 Algorithm Approach

The solution uses **backtracking**, a refined brute-force approach that:

1. **Place** a queen in a column
2. **Check** if the placement is safe
3. **Recurse** to the next column
4. **Backtrack** if no safe position is found
5. **Continue** until all queens are placed or all possibilities are exhausted

### Pseudocode Overview

```
function solveNQueens(board, column):
    if all queens are placed:
        return true
    
    for each row in current column:
        if position is safe:
            place queen
            if solveNQueens(board, next column):
                return true
            remove queen (backtrack)
    
    return false
```

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your system
- Basic understanding of recursion and backtracking (lecture PDF provided!)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/zain-cs/75-N-Queens-Problem.git
```

2. Navigate to the directory:
```bash
cd 75-N-Queens-Problem
```

## 💻 Usage

Run the Python script:

```bash
python "N-Queens Problem.py"
```

You can modify the value of N in the script to solve for different board sizes:

```python
# Example: Solve for 8-Queens problem
n = 8
solveNQueens(n)
```

## 📊 Complexity Analysis

- **Time Complexity**: O(N!)
  - In the worst case, we try to place N queens in N! different ways
  - Backtracking optimizes by pruning invalid branches early

- **Space Complexity**: O(N²)
  - Board representation requires N×N space
  - Recursion call stack depth is O(N)

## 🖼️ Example Output

For N = 4, one possible solution:

```
. Q . .
. . . Q
Q . . .
. . Q .
```

Where 'Q' represents a queen and '.' represents an empty cell.

## 📚 Learning Resources

This repository is perfect for:

- **Students** learning about backtracking algorithms
- **Interview preparation** for coding challenges
- **Algorithm enthusiasts** exploring classic computer science problems
- **Educators** looking for teaching materials

### Topics Covered

- Recursion and Backtracking
- Constraint Satisfaction Problems
- Algorithm Design and Analysis
- Chess and Board Games Logic
- Computational Complexity

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the code or add features:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

### Ideas for Contributions

- Add visualization of the solution
- Implement iterative approach
- Add more test cases
- Optimize for larger N values
- Create a GUI interface
- Add other solving algorithms (genetic algorithm, min-conflicts, etc.)

## 👨‍💻 Author

**Zain** - [@zain-cs](https://github.com/zain-cs)

Feel free to connect and explore more repositories!

## 📄 License

This project is open source and available for educational purposes. Feel free to use it for learning and teaching.

---

### 🌟 If you found this helpful, please consider giving it a star!

---

## 📞 Support

If you have any questions or suggestions, feel free to:
- Open an issue in this repository
- Reach out via GitHub

---

**Happy Coding! 🚀**
