[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"

# Deep RL Continuous Control Reacher
Udacity Deep Reinforcement Learning Nanodegree, second project "Continuous Control"

# Project 2: Continuous Control

### Environment

In this project, the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment with 20 agents is solved.
The goal is to move the robotic arms to a target location each.

![Trained Agent][image1]

### Rewards

In this environment, 20 double-jointed arms can move to target locations. A reward of +0.1 is provided for each step that one agent's hand is in the goal location. Thus, the goal of each arm is to maintain its position at the target locations for as many time steps as possible.
The environment is considered solved, when the average (over 100 episodes) of those average scores (of all the agents) is at least +30. 

### States and Actions

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of each arm. Each action (for one arm) is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.


### Files in this Repository
                    
    .
    ├── checkpoint_actor_128x128.pth          # stored weights for trained actor network (2 hidden 128 unit layers)
    ├── checkpoint_actor.pth                  # latest stored weights for trained actor network
    ├── checkpoint_critic_128x128.pth         # stored weights for trained critic network (2 hidden 128 unit layers)
    ├── checkpoint_critic.pth                 # latest stored weights for trained critic network
    ├── Continuous_Control.ipynb              # main code for training and testing the agent
    ├── ddpg_agent.py                         # agent to interact and learn from environment
    ├── model.py                              # neural network model (in Pytorch)
    ├── Report.pdf                            # report of the implementation and details of the learning algorithm
    └── README.md


### Python Packages
 
 - collections
 - copy
 - matplotlib
 - numpy
 - random
 - torch
 - unityagents
 
 **Note:** The Unity environment did not work on Mac OS for Python version 3.7 and higher. Python version 3.6 worked well.


### Downloading the Environment

You need only select the environment that matches your operating system:

Twenty (20) Agents:
 - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
 - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
 - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
 - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

Place the application in the same directory before executing.




(_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)


### Instructions

Follow the instructions in `Continuous_Control.ipynb` to get started with training your own agent!  











