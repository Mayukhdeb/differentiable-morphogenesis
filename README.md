# differentiable-morphogenesis
Implementing/experimenting with differentiable-morphogenesis (mostly neural cellular automata) on PyTorch

<code>
<img src = "images/bird.gif" width = "20%">
<img src = "images/lizard.gif" width = "20%">
<img src = "images/combined_infection.gif" width = "40%">

  </code>

### Notebooks:
| **Topic**                                                                                                                                      | **Link**                                                                                                                                                                                                      |
|------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Walkthrough of [Alexander Mordvintsev](https://twitter.com/zzznah)'s [youtube video](https://www.youtube.com/watch?v=8EN_8p9Toyc) on neural CA | [ ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/differentiable-morphogenesis/blob/main/notebooks/basic_walkthrough.ipynb)    |
| Cleaner implementation in case you just want to copy and paste stuff                                                                           | [ ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/differentiable-morphogenesis/blob/main/notebooks/nca_prototype.ipynb)        |
| [Experimental] Infection models                                                                                                                | [ ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mayukhdeb/differentiable-morphogenesis/blob/main/notebooks/infection_playground.ipynb) |

#### Important links:
* [Differentiable Self-organizing Systems thread on Distill](https://distill.pub/2020/selforg/)
* [Original Neural CA paper](https://distill.pub/2020/growing-ca/)
* [Another paper: Cellular automata as convolutional neural networks](https://arxiv.org/abs/1809.02942)

## A brief intro

A cellular automaton is a collection of cells on a grid of specified shape that evolves through a number of discrete time steps according to a set of rules based on the states of neighboring cells. The rules are then applied iteratively for as many time steps as desired.

Now let's ask the following question:

**What if we could use a neural network to map a certain set of rules  that would help us generate a very specific arrangement of "cells" ?**

That is exactly what our objective is. 

## Infection models

These models are trained to "infect" a given CA state 

Given a random point/set of points, the infection model's effect spreads through the image and turns it into something else. Apart from random starting points, they also work on both growing and grown states of the original CA. 

When I tried to recover the original image from a fully "infected" image, I ended up with a 4 legged abomination

<img src = "images/battle_fast.gif" width = "40%">


