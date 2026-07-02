# Alpha Ramp Pattern in C++

A beginner-friendly C++ program that demonstrates pattern printing using nested loops.

This project generates an **Alpha Ramp Pattern**, where each row contains the same uppercase alphabet repeated multiple times. The character changes with each new row, creating a visually appealing alphabetical pattern. It is a popular pattern-printing problem from Striver's A2Z DSA Sheet and helps strengthen understanding of nested loops and character manipulation.

---

## 📌 Features

* Prints an Alpha Ramp Pattern
* Uses nested `for` loops
* Demonstrates character manipulation using ASCII values
* Beginner-friendly implementation
* Helps improve logical thinking and pattern recognition skills

---

## 🛠️ Technologies Used

* C++
* Standard Library (`bits/stdc++.h`)

---

## 📂 Problem Statement

Given an integer `N`, print an alpha ramp pattern where each row contains the same uppercase letter repeated according to the row number.

### Example

For:

```txt
N = 5
```

Output:

```txt
A
BB
CCC
DDDD
EEEEE
```

---

## 📸 Screenshot

<img width="1210" height="786" alt="Screenshot 2026-07-02 132859" src="https://github.com/user-attachments/assets/3b68516c-f8fc-4826-8354-750548a0a6f7" />

Example folder structure:

```txt
project-folder/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
```

---

## 💻 Source Code

```cpp
#include <bits/stdc++.h>
using namespace std;

void alphaPattern(int n)
{
    for(int i = 0; i < n; i++) {

        char ch = 'A' + i;

        for(int j = 0; j <= i; j++) {
            cout << ch;
        }

        cout << endl;
    }
}
```

---

## ▶️ How to Run

1. Compile the program:

```bash
g++ main.cpp -o main
```

2. Run the executable:

```bash
./main
```

3. Enter the value of `N`.

---

## 📸 Example Output

### Input

```txt
4
```

### Output

```txt
A
BB
CCC
DDDD
```

---

## 📖 Learning Concepts

This project helps beginners understand:

* Nested loops
* Pattern printing
* Character (`char`) data type
* ASCII value manipulation
* Loop control statements
* Algorithmic thinking

---

## 🔍 Pattern Explanation

The pattern is generated using two nested loops.

### Outer Loop

Controls the number of rows.

```cpp
for(int i = 0; i < n; i++)
```

### Character Selection

The character for each row is calculated using:

```cpp
char ch = 'A' + i;
```

This produces:

* Row 1 → `A`
* Row 2 → `B`
* Row 3 → `C`
* Row 4 → `D`
* ...

### Inner Loop

Prints the selected character repeatedly.

```cpp
for(int j = 0; j <= i; j++)
```

The number of repetitions increases by one in each row, creating the Alpha Ramp Pattern.

---

## ⏱️ Complexity Analysis

### Time Complexity

```txt
O(N²)
```

The nested loops execute approximately **N²** iterations.

### Space Complexity

```txt
O(1)
```

The program uses only loop variables and does not require additional memory.

---

## 👨‍💻 Author

Developed as a beginner-friendly C++ practice project for learning nested loops, character manipulation, and pattern printing.
