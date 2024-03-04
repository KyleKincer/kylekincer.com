---
title: Solvataire
date: 2024/03/03
description: A brute-force solver for the game Peg Solitaire in Rust. 
tag: Rust
author: Kyle Kincer
---
# Solvataire
### A Peg Solitaire Solver
If you're anything like me, you've been called an [**eg-no-ra-moose**](https://blog.crackerbarrel.com/2021/08/13/how-to-beat-the-cracker-barrel-peg-game/) by that silly peg game at Cracker Barrel one too many times. I'd had enough.

Solvataire is a brute-force solver for the game [Peg Solitaire](https://en.wikipedia.org/wiki/Peg_solitaire), written in Rust. It uses a recursive depth-first search to solve the game. Currently only implemented for the triangle board commonly found at Cracker Barrel™️ restaurants, but I plan to support the English boards at some point. 

### Links
- [GitHub](https://github.com/KyleKincer/solvataire)

## Implementation
### Algorithm
The solver uses a recursive backtracking algorithm to find the shortest sequence of moves to solve the game. It starts with an initial board state and explores all possible moves from that state, recursively searching until it finds a solution. 

### Performance
The solver is multithreaded, using Rust's `rayon` library to parallelize the search. 