# differentiable-morphogenesis
> Implementing/experimenting with differentiable-morphogenesis (mostly neural cellular automata) on PyTorch

#### Important links:
* [Differentiable Self-organizing Systems thread on Distill](https://distill.pub/2020/selforg/)
* [Original Neural CA paper](https://distill.pub/2020/growing-ca/)
* [Another paper: Cellular automata as convolutional neural networks](https://arxiv.org/abs/1809.02942)

## A brief intro

A cellular automaton is a collection of cells on a grid of specified shape that evolves through a number of discrete time steps according to a set of rules based on the states of neighboring cells. The rules are then applied iteratively for as many time steps as desired.

Now let's ask the following question:

**What if we could use a neural network to map a certain set of rules  that would help us generate a very specific arrangement of "cells" ?**

That is exactly what our objective is. 

