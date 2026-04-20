# Word Ladder Game & Solver

## Description
This project is a high-performance C program designed to solve the classic "Word Ladder" puzzle. The goal is to find the shortest possible transformation from a starting word to a target word by changing only one letter at a time. Each step must be a valid word found in the provided dictionary. I built this to demonstrate efficient graph traversal techniques and to practice managing complex data structures in a low-level language.

## Features
* **Shortest Path Guarantee:** By utilizing a Breadth-First Search (BFS) algorithm, the program always identifies the most efficient transformation sequence.
* **Dictionary Validation:** The solver dynamically loads and parses a dictionary file to ensure every step in the ladder is a legitimate word.
* **Robust Error Handling:** The program effectively detects and reports scenarios where a word ladder is impossible, such as when words are of different lengths or no path exists.
* **Memory Management:** Includes a full cleanup routine to ensure no memory leaks occur during dictionary loading or path searching.

## Tech Stack
* **Language:** C
* **Algorithms:** Breadth-First Search (BFS)
* **Tools:** Makefiles, GDB, Valgrind

## Timeline
* **Setup:** Wrote code to load and store words from a dictionary file.
* **Build:** Created functions to find "neighbor" words (words only one letter away).
* **Search:** Implemented the BFS logic to guarantee the shortest transformation path.
* **Cleanup:** Fixed logic bugs, added a Makefile, and ensured all allocated memory is properly freed.

## Challenges
* **Performance:** Optimized the search logic to prevent lagging or crashing when using dictionaries with thousands of words.
* **Path Reconstruction:** Managed the queue and data structures to ensure the program remembers and prints the final ladder in the correct order.
