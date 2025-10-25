In this project, I implement a solver that fills in the unknown entries in an N x N sudoku or latin square. Using Grover's alogrithm allows quantum computers to solve this kind of problem more quickly than a classical computer is able to for a large number of unknown values.

In this notebook, I design all the quantum gates needed to properly implement Grover's alogrithm, and explain the ways that the problem of solving a soduko/latin square is mapped to an application of Grover's algorithm.

The notebook culminates with a function "solve_puzzle" whose input is an array of size N x N (for N any positive integer), whose entries are the digits 0,...,N-1 for the "known" spaces in the puzzle, and 'None' for the "unknown" spaces in the puzzle. There are also two optional Boolean parameters "decompose" which uses my implementation of a multicontrolled X gate when True, and the built-in Qiskit version when False (this makes it possible to run larger puzzles on a home computer when set to False). The second optional Boolean is "showPlot", which will return the probabilities of all possible computational basis outputs in the final state after the code is run.

The code returns a list of integers in {0,...,N-1} corresponding to the (likely) entries for the unknown spaces in the puzzle, in order from left to right & top to bottom.
