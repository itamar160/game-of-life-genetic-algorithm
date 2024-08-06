# game-of-life-genetic-algorithm
this genetic algorithm aims to find a methuselah that grows the most in the game of life.

Game of Life:
The game of life is a zero-player game, meaning that its evolution is determined by its initial state, requiring no further input. 
One interacts with the Game of Life by creating an initial configuration and observing how it evolves. 

Rules:
The universe of the Game of Life is an infinite, two-dimensional orthogonal grid of square cells, each of which is in one of two possible states, live or dead (or populated and unpopulated, respectively). 
Every cell interacts with its eight neighbors, which are the cells that are horizontally, vertically, or diagonally adjacent. At each step in time, the following transitions occur:
1) Any live cell with fewer than two live neighbours dies, as if by underpopulation.
2) Any live cell with two or three live neighbours lives on to the next generation.
3) Any live cell with more than three live neighbours dies, as if by overpopulation.
4) Any dead cell with exactly three live neighbours becomes a live cell, as if by reproduction.

Methuselah:
A methuselah is a pattern that takes a large number of generations in order to stabilize (known as its lifespan) and becomes much larger than its initial configuration at some point during its evolution.
A pattern stabilizing means that it enters into a loop.

Genetic Algorithm:
In computer science and operations research, a genetic algorithm (GA) is a metaheuristic inspired by the process of natural selection that belongs to the larger class of evolutionary algorithms (EA). 
Genetic algorithms are commonly used to generate high-quality solutions to optimization and search problems by relying on biologically inspired operators such as mutation, crossover and selection.
In a genetic algorithm, a population of candidate solutions to an optimization problem is evolved toward better solutions. 
Each candidate solution has a set of properties (chromosomes) which can be mutated and altered.

A genetic algorithm requires:
1) a representation of the solution domain - in our case a set of all the coordinates of the live cells in the first generation of the game/chromosome.
2) a fitness function to evaluate the solution domain - We define a methuselah's fitness as it's maximum size divided by it's intial size.

Interm solutions that the genetic algorithm finds are shown to the user via tkinter.
