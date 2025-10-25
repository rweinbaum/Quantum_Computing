# BooleanQuantumROM

In this notebook, I implement a more efficient Boolean Quantum ROM. Given any function with n-binary inputs f(x_0,...,x_{n-1}) that outputs a 0 or 1, the final function U_f(f,n) designs quantum circuit that implements f via |x_0...x_{n-1}0> -> |x_0...x_{n-1}f(x_0,...x_{n-1})>.

I begin with the most straightforward, but inefficient, implementation of such a circuit. I then discuss two simplifications that we can perform to make our circuit more efficient. In the following section I implement both simplifications, and then tie the two simplifications together in the final section. The result is a function U_f(f,n) that creates the quantum circuit implementing f.

To use this function, start by defining a Python function f whose input is a list of length N consisting of 0's and 1's, and whose output is either 0 or 1. Calling U_f(f,N) will return a quantum circuit implementing f as above.
