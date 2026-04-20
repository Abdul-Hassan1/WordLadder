Word Ladder Game & Solver

Description:
This project is a high-performance C program designed to solve the classic "Word Ladder" puzzle. The goal is to find the shortest possible transformation from a starting word to a target word by changing only one letter at a time. 
Each  step must be a valid word found in the provided dictionary. I built this to demonstrate efficient graph traversal techniques and to practice managing complex data structures in a low level language.

Features
Shortest Path Guarantee: By utilizing a Breadth-First Search (BFS) algorithm, the program always identifies the most efficient transformation sequence.

Dictionary Validation: The solver dynamically loads and parses a dictionary file to ensure every step in the ladder is a legitimate word.

Robust Error Handling: The program effectively detects and reports scenarios where a word ladder is impossible, such as when words are of different lengths or no path exists.

Memory Management: Includes a full cleanup routine to ensure no memory leaks occur during dictionary loading or path searching.

Tech Stack
Language: C

Algorithms: Breadth-First Search (BFS)

Data Structures: Queues, Linked Lists/Graphs

Tools: Makefiles for build automation, GDB for debugging, Valgrind for memory leak detection

Timeline
Initial Setup: The project began with building a robust file parser to load the dictionary into memory efficiently.

Core Logic Development: I developed helper functions to identify "neighbor" words—words that differ by exactly one character—to build the connections between potential ladder steps.

Search Implementation: I integrated a BFS algorithm using a queue-based system to explore all possible word transformations layer by layer.

Refinement & Cleanup: The final phase involved optimizing the search speed, automating the build process with a Makefile, and verifying memory safety using Valgrind.

Challenges
Optimizing Search Speed: One of the biggest hurdles was ensuring the search didn't lag or crash when processing dictionaries with tens of thousands of words. I had to optimize how neighbors were identified to maintain performance.

Path Reconstruction: Ensuring the program could accurately track and print the steps of the ladder in the correct order required careful management of the queue data structure and parent-node tracking.
