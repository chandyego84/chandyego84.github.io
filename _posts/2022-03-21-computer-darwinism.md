---
layout: post
title: Self-Driving Simulation Based on Darwinism
---
### Introduction
The goal of this projec was to simulate a "self-driving" car in the Unity engine using neural networks and the genetic algorithm. The neural network was used to navigate through the track and was trained or optimized through an evolutionary process. Given a predefined path, the car's ability to drive itself was primarily based on how far it was able to move along the track without hitting another object or steering off to the side of the track. To add some more complexity, I ensured that the car had to take slight turns. 

### Neural Networks
Neural networks are the core of deep learning algorithms and both their name and structure are inspired by the human brain. The neural network is a collection of neurons that are connected to each other and can be trained to learn patterns in data. They rely on data to learn and improve their acuracy over time. The network consists of an input layer where the value from each input node travels through the arbitrary amount of hidden layers, and then finally through the output nodes to produce some results. Each node produces an output based on the connections from the previous layer (weights) and some bias, and can be described shortly by an activation function which sums the product of the weights and the corresponding node values attached to the weights, plus a bias value.If you want to learn more, this [project on recognizing handwritten digits](http://neuralnetworksanddeeplearning.com/chap1.html) is a good place to start.

![NN vs Brain](/assets/img/NNandBrain.png)

### Genetic Algorithm
As stated, the neural network needs to be trained in order to produce desired results which should allow the car to nabigate through the track. The genetic algorithm is a heuristic evolutionary process inspired by the process of natural selection. Genetic algorithms are typically used to solve optimization or search problems, where in this case the neural network is being optimized to produce the best outputs for the car to travel through the track. Again, for more learning, this [article](https://medium.com/@AnasBrital98/genetic-algorithm-explained-76dfbc5de85d) is a good place to start.

There are variations to each step, but the main algorithm is as follows:
1. Create a population of random individuals (set of cars with random neural networks and random weights)
2. Evaluate the fitness of each individual
3. Select the best performing or fittest individuals for the next generation
4. Create a new generation of individuals using crossover and mutation
5. Repeat steps 2-4 until the desired number of generations is reached

### Implementation

### Conclusion