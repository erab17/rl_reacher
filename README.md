# Reacher Project



## Introduction
In this project 20 agents will be trained to keep their arm within a specific target zone and keep it there throughout time. Each agent have a double-jointed arm.... The agent recieves a +0.1 reward for every time step that the arm is withing the goal zone. 

The state space consists of 26 different states for each which consists of position, rotation, velocity and angular velocities. For the action space there are four continous actions between -1 and +1 that corresponds to the torque to two joints.

In the below gif we can see the 20 different agents and their arms and their respective target zones.
![hippo](https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif)

If no time step restriction is set the agent will run for about 1000 timesteps before terminating.
 
The target for the agents is to achieve a rolling reward over 100 episodes of 30 or more of an average of all the agents.

## Libraries needed
The following libraries need to imported in order to run all the cells in the notebook
* UnityEnvironment from unityagents  
* numpy  
* random  
* namedtuple and deque from collections  
* torch  
* matplotlib
* import pickle
* pandas
* copy

## Running the agent
To run the agent in the environment and using the different methods one just have to sequantially execute the cells in the notebook. 

The function "ddpg" runs the training phase of the networks if nothing else is specified it will for 400 episodes. Before this function is run one also needs to instatiate the StoreResults class which helps with saving some results from the run. In addition the Agent has to be instatiated as well before running the training function.
