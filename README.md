# Tideman Voting System

This project implements the **Tideman voting algorithm** (also known as the "Ranked Pairs" method) in C. It's designed to determine the winner of an election based on voters' ranked preferences — avoiding major pitfalls of other systems like plurality voting.

## How It Works

1. Voters rank candidates in order of preference.
2. Preferences are recorded pairwise between every candidate.
3. Pairs of candidates are sorted by strength of victory.
4. Pairs are locked into a directed graph — avoiding cycles.
5. The source of the graph is declared the winner.

## Getting Started

### Prerequisites

- GCC or Clang compiler
- Terminal access (Linux/Mac/WSL/Git Bash on Windows)
- CS50 Library (optional — see below)

### Compilation & Execution

To compile and run:

bash
clang -o tideman tideman.c -lcs50  # If using CS50
./tideman Alice Bob Charlie        # Replace with candidate names

#### Acknowledgements
This project was originally developed as part of CS50: Introduction to Computer Science offered by Harvard University.
