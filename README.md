# 15‑Puzzle — C++ Implementation

A carefully crafted implementation of the classic 15‑puzzle (sliding puzzle) in C++. The 15‑puzzle challenges you to arrange the numbers 1–15 in a 4×4 grid by sliding tiles into the empty space. This repository contains an implementation that lets you play, experiment with shuffles, and inspect or extend the solver logic.

## Table of Contents
- [About](#about)
- [Features](#features)
- [How it works (brief)](#how-it-works-brief)
- [Build & Run](#build--run)
- [Usage](#usage)
- [Examples](#examples)
- [Extending & Contributing](#extending--contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## About
The 15‑puzzle is a deceptively simple yet fascinating problem that illustrates search, heuristics, and state‑space reasoning. This project provides a readable and approachable codebase so you can:
- Play the puzzle from the terminal,
- Observe different starting configurations,
- Study or extend the solver code (if included) to experiment with heuristics and search strategies.

## Features
- Clean, commented C++ code (modern C++ recommended).
- CLI interface for interactive play and testing.
- Utilities for generating solvable shuffles / loading custom board states.
- Clear structure so you can add search algorithms (A*, IDA*, BFS) or visualizations.

## How it works (brief)
- The board is a 4×4 grid with tiles 1–15 and one empty slot.
- A move slides a tile adjacent to the empty slot into it.
- Common solver approaches include A* search with admissible heuristics like the Manhattan distance, but you can swap or add algorithms in the codebase to compare performance and solution length.

## Build & Run
Requirements:
- A C++ compiler supporting C++11 or later (g++, clang++)

Compile (example):
```bash
# If your main file is main.cpp or there are multiple .cpp files:
g++ -std=c++17 -O2 -Wall *.cpp -o fifteen
# Or, for a single-file build:
g++ -std=c++17 -O2 -Wall main.cpp -o fifteen
