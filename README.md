# Microsoft Boggle Solver

A simple C++ implementation of the classic Boggle word‐finding game using a Trie (prefix tree) for fast dictionary lookups. Given an _N_×_M_ grid of letters and a word list (`dictionary.txt`), the solver finds all valid words that can be formed by chaining adjacent letters (including diagonals) without reusing the same cell in a single word.

---

## Table of Contents

- [Features](#features)  
- [Files](#files)  
- [Prerequisites](#prerequisites)  
- [Building](#building)  
- [Usage](#usage)
  
---

## Features

- **Fast lookup** via a Trie data structure  
- Supports arbitrary board sizes (_N_×_M_)  
- Searches in all 8 directions (horizontal, vertical, diagonal)  
- Reports:
  - List of valid words found  
  - Total count of words  
  - Time taken (in milliseconds)  

---

## Files

| File             | Description                                                  |
| ---------------- | ------------------------------------------------------------ |
| `boggle.cpp`     | Main solver implementation (builds Trie, performs DFS search) |
| `trie.h`         | Header-only Trie class (insert, search, delete operations)  |
| `dictionary.txt` | Newline‑separated list of lowercase words for the solver     |
| `Boggle.out`     | Compiled executable (generated after building)               |

---

## Prerequisites

- A C++ compiler with C++11 (or later) support  
- Standard C++ library  
- ~10 MB of RAM for large dictionaries (e.g., 100 K–200 K words)

---

## Building

```bash
# Compile the solver
g++ -std=c++11 boggle.cpp -o Boggle.out
```
## Usage 
- Prepare your `dictionary.txt` in the same folder (one lowercase word per line).
- Run the solver : 
     ```bash
     ./Boggle.out
     ```
- Follow Prompts :
     ```bash
    Enter number of rows and cols
    4 4
    Enter board values of 4 by 4
    abcd
    efgh
    ijkl
    mnop
     ```
- Output :
  - List of all valid words found on the board
  - Total number of words
  - Execution time in milliseconds
 

