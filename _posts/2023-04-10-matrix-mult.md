---
title: 'Matrix Multiplication: Resurrections'
date: 2023-04-10
permalink: /blog/2023/03/matrix-mult/
tags:
  - research
---
*An understated breakthrough in AI research.*

On October 5th, the research group DeepMind resurrected a 50-year line of work on the computational efficiency of matrix multiplication -- a fundamental calculation at the heart of all procedures in computer science. In their latest Nature publication, DeepMind demonstrated that an artificially intelligent (AI) system can make mathematical discoveries and break barriers researchers previously thought were impenetrable, showcasing a staggering achievement for AI as it continues to surpass human intuition.

The problem of matrix multiplication is at the core of all computer processes. A matrix is a grid of numbers that can abstractly represent essentially anything, and their multiplication is representative of some change in that representation. For example, analyzing an MRI scan is reliant upon thousands and thousands of matrix multiplications. As such, it is of immense value to find the fastest method for conducting this higher-dimensional arithmetic -- one which will reduce the cost of running on a computer and, as a result, save energy.

The costliest, or most time-consuming, mathematical procedure done on any classical computer is multiplication, which is inherently a recursive summation of numbers. Therefore, the cost of any large-scale computation is dictated by the number of multiplications one must compute. Consider the simple equation

$$x^2 - y^2$$

which contains two multiplications (tucked into the exponents) and a subtraction. To reduce the cost incurred in calculating this value, we can rewrite the expression as 

$$(x+y)(x-y)$$

to obtain the exact same value with only one multiplication, thus incurring a lower cost. 

This is precisely the insight Volker Strassen, a German mathematician at the University of Konstanz, had in 1969 when he recognized that the standard approach to computing the multiplication of two matrices is suboptimal. His algorithm which utilized the above idea required only a fraction of the cost to implement when compared to the naive method. While Strassen's algorithm is by no means fast, it broke the barrier and left computer scientists with a fascinating new question to explore: can we do even better?

It's been 53 years since Strassen invented his algorithm and we still don't know the answer to this question. Or rather, we didn't know until the publication of AlphaTensor in the journal Nature just a few months ago. This algorithm builds upon DeepMind's prior work that trained an AI, dubbed AlphaZero, to play Chess and Go at a superhuman level via reinforcement learning: a teaching method that uses rewards and punishments for each move selected in the game to correct behavior. By reformulating the matrix multiplication task as a sort of three-dimensional board game where moves are representative of different calculations, AlphaTensor learned to play the game by receiving a reward for winning in as few moves as possible. Over the course of the learning procedure, the AI sifted through over 1033 possible ways of multiplying to find the fastest sequence of moves which resulted in a novel algorithm. During the learning process, AlphaTensor even rediscovered Strassen's algorithm before identifying further improvements to the procedure. Within a matter of minutes, this artificially intelligent system was uncovering the best-known algorithms before electing to discard them in favor of further refinements that no human had previously imagined.

After learning to play this game-formulation of the desired computation, AlphaTensor discovered an algorithm that either matched the best-known human designed procedure or improved upon it in all problem settings. For example, multiplying a 4-by-5 matrix with a 5-by-4 matrix requires 100 individual multiplications in the naive algorithm, and the best human-designed algorithm to date reduced this to 80 -- AlphaTensor discovered an algorithm requiring only 76. While this improvement may feel marginal, when the procedure is implemented across thousands upon thousands of matrices, the improvement becomes an exponential discrepancy. 

Much like in 1969 when Strassen opened a world of curiosities on a seemingly uninteresting problem, the DeepMind group have decidedly pushed the goal posts forward and invited the research community to continue this effort. More importantly still, this result establishes AI as a ubiquitous tool in accelerating our incessant prodding at several unresolved problems in the field -- a symbiotic approach to computer science.
