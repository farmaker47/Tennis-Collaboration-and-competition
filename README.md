# Tennis-Collaboration-and-competition
In this AI environment, two agents control rackets to bounce a ball over a net.

This project is an implementation of AI Gym's [tennis environment](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis)


![](tennis.gif)

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single score for each episode.

The environment is considered solved, when the average (over 100 episodes) of those scores is at least +0.5.

## Installation

1. Download the environment from one of the links below. You need to select only the environment for your operating system:

- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)

(For Windows users) Check out this [link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not enabled a [virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use this [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the root folder, and unzip (or decompress) the file.

3. Make sure you install Anaconda. You can download it from [here](https://www.anaconda.com/distribution/)

4. Now you can create your environment. Lets call our environment ```DRLND```
  
   Linux,Mac
   ```
   conda create --name drlnd python=3.6
   source activate drlnd
   ```
   Windows
   ```
   conda create --name drlnd python=3.6 
   activate drlnd
   ```
 5. We will be working with pytorch version 0.4.0 (an early version), so make sure that you install this version of pytorch:
   ```
   conda install pytorch=0.4.0 -c pytorch
   ```
 6. Perform a minimal installation of the [OpenAI Gym environment](https://github.com/openai/gym)
 
 7. Use command ```pip install``` and use it with all dependencies of the requirements.txt file
 
 8. Create a Python execution backend for Jupyter for the drlnd environment 
   ```
   python -m ipykernel install --user --name drlnd --display-name "drlnd"
   ```
 AND you are ready to use the environments

## Instructions
Follow the instructions in ```Tennis_Soloupis_final.ipynb``` to get started with training your agents!

## Run the code
Execute the cells inside ```Tennis_Soloupis_final.ipynb``` file in sequential order so to proceed with training the agents. Tweak the hyperparameters to get different results. Using GPU gives 4 times faster results.
