# rl_reacher

Project Details

The README describes the the project environment details (i.e., the state and action spaces, and when the environment is considered solved).



Getting Started

The README has instructions for installing dependencies or downloading needed files.

Instructions

The README describes how to run the code in the repository, to train the agent. For additional resources on creating READMEs or using Markdown, see here and here.



## Introduction
In this project 20 agents will be trained to keep their arm within a specific zone. The agents job is to keep it's arm in the specifiz zone. The yellow bananas give a +1 reward whereas the blue bananas give a -1 reward.

![hippo](https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif)

The agent can take four different actions:
- Move forward.
- Move backward.
- Move left.
- Move right.

The state space consists of 37 different states including velocity and the ray tracing perception of the agent's forward field of view. 

This is an episodic task becuase the episode will automaticly end after 299 time steps.

## Libraries needed
The following libraries need to imported in order to run all the cells in the notebook
-- UnityEnvironment from unityagents  
-- numpy  
-- random  
-- namedtuple and deque from collections  
-- torch  
-- matplotlib.pyplot  
-- pandas as pd  

## Running the agent
To run the agent in the environment and using the different methods one just have to sequantially execute the cells in the notebook. 

All the different methods are in the notebook. However, the code needs to be refractored becuase in order to run the different methods one as to manually do some comment and uncomment in the correct places. The code in its default will run a DQN with eperience replay using softmax with decaying temperature for action selection.
