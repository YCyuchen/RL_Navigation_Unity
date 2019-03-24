# RL_Navigation_Unity
This repo is an implement of Unity's [Banana Navigation](https://github.com/Unity-Technologies/ml-agents) with Deep Q-learning Network

-------
### Overview
![banana](https://github.com/YCyuchen/RL_Navigation_Unity/blob/master/banana.jpg)


&emsp;In this project, an agent is trained to collect yellow banana in a large square world. A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

   
### Depedency
- python 3.6
- [ml-agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) from Unity
- Numpy
- pytorch(0.4.0)

# Project Deatil
Here are the environment details from Unity
```        Vector Observation space type: continuous
        Vector Observation space size (per agent): 37
        Number of stacked Vector Observation: 1
        Vector Action space type: discrete
        Vector Action space size (per agent): 4
        Vector Action descriptions: , , , 
```
The space has 37 dimensions containing the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Action space  has 4 dimensions, corresponding to:
&emsp;&emsp;**0**: move forward.  
&emsp;&emsp;**1**: move backward.  
&emsp;&emsp;**2**: turn left.  
&emsp;&emsp;**0**: turn right.  

## Get started
File model.py contains the network for Q-learning and dqn_agent contains policy for agent to make action.

Run Navigation.ipynb to see the details.
