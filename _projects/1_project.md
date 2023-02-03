---
layout: page
title: Minimize Surprise
description: Evolution of swarm robot controllers 
img: assets/img/MinimizeSurprise.jpg
importance: 1
---



Robot swarms are decentralized collective systems of simple embodied agents that act autonomously and rely on local information only. Such large-scale multi-robot systems can be beneficial over single robots due to higher potential for robustness and scalability. However, the development of swarm robot controllers is challenging because when implementing a desired swarm behavior one has to take into account hard-to-anticipate local interactions between robots and between robots and the environment. An alternative is the automatic design of swarm robot controllers using methods of evolutionary robotics. 
Since evolutionary algorithms maximize fitness potentially by every possible way, undesired side effects may occur if a goal-directed fitness function was not specified accurately enough. By contrast, task-independent fitness functions avoid the specific formulation of rewards but do not guarantee that desired behaviors emerge. 

Our minimize surprise approach relies on such a task-independent fitness function to evolve diverse collective behaviors for robot swarms. 
Surprise, in its simplest form here, is the difference between observed and predicted sensor values. 
We minimize surprise over generations by equipping each swarm member with an actor-predictor pair of artificial neural networks and putting direct selection pressure on the predictor. 
The actor is only indirectly rewarded by being paired with the predictor and thus swarm behaviors emerge as a desired by-product. 

The emergened swarm behaviors have proven to be diverse, robust, and scalable. 
The generated behavioral diversity is competitive to state-of-the-art diversity methods, such as novelty search, and the combination of minimize surprise with MAP-Elites leads to behavioral diversity within and across tasks. 
Furtermore, using minimize surprise for online evolution enables robots to adapt to changes in their environment. 

We have evolved swarm robot controllers for a variety of scenarios: self-assembly, basic swarm behaviors, collective construction, collective perception, and object manipulation.
Our experiments were conducted in simple simulations, advanced simulators, and on physical robots. 
In future work, we aim to target more complex scenarios and environments. 

An overview of our results can be found in our T-RO journal article <a href="https://ieeexplore.ieee.org/document/9813360/references#references">Innate Motivation for Robot Swarms by Minimizing Surprise: From Simple Simulations to Real-World Experiments</a>.
The code of our experiments is available on <a href="https://github.com/minimize-surprise">GitHub</a>.
