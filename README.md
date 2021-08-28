# Udacity-DQN-Navigation
 This repository contains a simple solution to Udacity's [Navigation project](https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation). The remaining sections of the README describe how to train and test the agent as well as the overall structure of the algorithm used to solve the problem. 
 
 ## Introduction
 ### The Environment
The description of this environment is taken from the Udacity Navigation Project lecture. In this project, an agent learns to navigate and collect banans in a large square world. **The agent gains a reward of +1 when it collects a yellow banana and a reward of -1 when it collects a blue banana.** **The goal of this agent is to maximize the number of yellow bananas while avoiding blue bananas. **

### State Space
**The state of the environment at each timestep is a 37-dimensional vector**. This state consists of the agent's velocity and ray-based perception of objects in front of the agent. The agent also has a **set of 4 discrete actions** corresponding to:
* 0 - Move forward
* 1 - Move backward
* 2 - Move left
* 3 - Move right

### Success criteria
The environment is considered solved when the agent obtains a score of > 13 over 100 consecutive episodes of the task.

## Getting started
Please follow the instructions to get started at [Udacity's Navigation Project github page](https://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigationhttps://github.com/udacity/deep-reinforcement-learning/tree/master/p1_navigation). **Alternatively, if executing the project in a Udacity workspace, it is sufficient to run the notebooks which will install all relevant requirements via pip inline in the notebooks.**

### Training the agent
In order to train the agent, **please go through the training cells in** ```Navigation-Training.ipynb```. The result of the training is the checkpoint.pth file which stores the weights of the trained Q-Network. The pretrained notebook lists all the executed steps taken to train the network. 

### Testing the agent
In order to test the agent, **please go through the testing cells in** ```Navigation-Testing.ipynb```. Ensure that a valid ```checkpoint.pth``` is present in the same folder as the notebook. My solution checkpoint is included in this repository. The cells in this notebook will run the agent in the environment till the simulation is ```done```. The agent easily achieves an average score of > 13 over 100 episodes. 

## Acknowledgments
The skeleton code for the deep-q-learning agent and associated model borrows heavily from [Udacity's example deep-q-learning agent lesson](https://github.com/udacity/deep-reinforcement-learning/tree/master/dqn). My solution builds on top of the provided files. 
