
# Udacity Deep Reinforcement Learning Project 1: Navigation

### Introduction

For this project, I trained a reinforcment learning agent to navigate within a large, square world modeled in Unity, avoid blue bananas in this space, and collect yellow bananas.  

A reward of +1 was provided for collecting a yellow banana, and a reward of -1 was provided for collecting a blue banana.  The goal of my agent was to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions that includes the agent's velocity and ray-based perception of objects in front of the agent.  Given this information, the agent was trained to select an optimal set of actions.  Four different actions are available, corresponding to the following four int values:
- **0** - move forward.
- **1** - move backward.
- **2** - turn left.
- **3** - turn right.

The task consisted of a series of episodes (the number of which was a hyper-parameter) , and in order to solve the environment, my agent was required to achieve an average score of +13 or better over 100 consecutive episodes.  The final implementation achieved a score of 15.46 after executing 5,000 episodes of interacting with the environment.

### Setting Up the Environment

#### Unity ML-Agents
The Unity game engine team has developed a programming environment specifically designed to support intelligent agent programming.   The unity environment was used to create a playing area and populate it with yellow and blue bananas.  To execute the code in this project, you will first need to download and install the Unity ML-Agents code library.  The following steps were provided by the Udacity team and will result in a complete environment capable of executing this project.

1. Follow the [instructions](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) to install Unity ML-Agents. 

2. Navigate to the `p1_navigation/` folder, and run the command below to obtain a few more packages.
  ```
  pip3 install -r requirements.txt
  ```

3. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

4. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 

### Instructions

The main file of this project is `Navigation.ipynb`. To use a Jupyter notebook, run the following command from the `p1_navigation/` folder:
```
jupyter notebook
```
and open `Navigation.ipynb` from the list of files.  Alternatively, you may prefer to work with the [JupyterLab](https://jupyterlab.readthedocs.io/en/latest/) interface.  To do this, run this command instead:
```
jupyter-lab
```

Once the project notebook has been opened, you can simply click the "Run->" button in the main menu to execute the python program that opens the Unity banana playing field and starts to train an agent to navigate this environment.
