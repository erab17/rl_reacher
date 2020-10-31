# rl_reacher

Project Details

The README describes the the project environment details (i.e., the state and action spaces, and when the environment is considered solved).



Getting Started

The README has instructions for installing dependencies or downloading needed files.

Instructions

The README describes how to run the code in the repository, to train the agent. For additional resources on creating READMEs or using Markdown, see here and here.



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

## Running the agent
To run the agent in the environment and using the different methods one just have to sequantially execute the cells in the notebook. 

All the different methods are in the notebook. However, the code needs to be refractored becuase in order to run the different methods one as to manually do some comment and uncomment in the correct places. The code in its default will run a DQN with eperience replay using softmax with decaying temperature for action selection.
