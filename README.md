# N-Queens-Problem-Genetic-Algorithm
A mono-objective genetic algorithm to solve the N-Queens Problem. Coded in Python on Jupyter Notebook.

## N-Queens Problem
Given a regular chessboard (NxN dimensions) and N queens, the problem with N-queens is to reallocate
them on the chess in a way that no queen may capture another queen.

The problem can be formulated as a classical Constraint satisfaction problem, whose goal is to find a
configuration of the queens in the board that does not violate any constraints.

In order to solve this problem by using Genetic Algorithms (GA) we must first define:
> a representation (codification) for the individuals (i.e. candidate solution);
> 
> a fitness function to evaluate the performance of a candidate solution;
> 
> one or more genetic variation operator;
> 
> one or more selection mechanism;
> 
> a stop criteria, for example, either generation number or a fitness value.

## 🔨 The Genetic Algorithm
The algorithm is an implementation of a mono-objective genetic algorithm and is explained through the comments I put along the code.

Initially I tried a strategy of starting with an empty board and inserting queens randomly as long as it didn't violate any constraints. This way, the population had only valid individuals and the fitness function to be maximized was the number of queens on the board. With this strategy, I found that the algorithm quickly reached a situation with 7 queens on the board but struggled to evolve to a board with 8 queens. After experimenting with the parameters of this strategy, I noticed that a large number of individuals (1000) was needed for the algorithm to converge to 8 queens.

So, I changed the strategy so that all individuals in the generation had 8 queens and the fitness function to be minimized became the number of collisions between the queens. In this new strategy, the algorithm behaved more efficiently, finding a valid position with 8 queens faster. * As the delivered version is changed, it has some functions that are no longer used, but are illustrative to demonstrate the evolution of the adopted strategy.

With the exercise, it became clear that the strategy used to generate individuals and calculate fitness influences the convergence capacity of the genetic algorithm, and a strategy may have better results depending on each problem addressed.

## How to run the code

This is a Python implantation. In order to keep it easy, I did it using Jupyter Notebook. Just download the “N-Queens Problem Genetic Algorithm.ipynb” file, and run it on Jupyter Notebook.

Feel free to ask questions and contribute.

## Autor

| [<img src="https://avatars.githubusercontent.com/u/33962854?v=4" width=115><br><sub>Celso Meireles</sub>](https://github.com/CelsoMeireles) 
| :---: | 
