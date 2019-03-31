# continuous-control-rl
An RL agent that solves Unity's Reacher environment for a continuous control task 

## Project Details:
**Overview:** 
Broad goal is to train an agent to successfully solve Unity's Reacher environment.

**Goal & Rewards:** 
A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of the agent is to maintian its position at the target location for as many time steps as possible. 

**State Space:** 
The state space has 33 dimensions and contains the arm's position, rotation, velocity, and angular velocities.

**Action Space:**
Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

**Solving condition:**
The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

## Getting Started:
### Setting up the python environment and installing dependencies
 1. Create (and activate) a new environment with Python 3.6.

   - Linux or Mac:
 
      `conda create --name continuous_control python=3.6`
      `source activate continous_control`
      
   - Windows:
   
     `conda create --name continuous_control python=3.6`  
     
     `activate continuous_control`
  
 2. Clone the repository, Then, install several dependencies.
 
     `git clone https://github.com/ramanshrivastava/continuous-control-rl.git`
     
     `pip install -r requirements.txt`
     
     
 3. Create an IPython kernel for the `continuous_control` environment.
 
    `python -m ipykernel install --user --name continuous_control --display-name "continuous_control"`
   

 4. Before running code in a notebook, change the kernel to match the `continuous_control` environment by using the drop-down Kernel menu.

### Download the Unity Environment 
1. Download the environment from one of the links below. You need only select the environment that matches your operating system:

  - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
  - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
  - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
  - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

(For Windows users) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

(For AWS) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the `continuous-control-rl` GitHub repository, in the root folder, and unzip (or decompress) the file.


## Instructions:
1. Open the `Continuous_Control (1).ipynb` jupyter notebook and execute each code cell to train the agent. 
2. Once the necessary packages are imported as a next step provide the `file_name` for the `UnityEnvironment`
3. Execute the rest of the cells as it is there after 
4. provide the `PATH` for `.pth` files in the code cell 8 to save actor and critic model weights. 
