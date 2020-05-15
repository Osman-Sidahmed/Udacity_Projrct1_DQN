# Udacity_RL_01
## Navigation project

### About the Project
The goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.The environment state is described by 37 variables among which the agent's velocity, along with ray-based perception of objects around the agent's forward direction. The agent has to learn the best strategy that defined the best action for any given environment state. Agent actions are discrete corresponding to:

0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right.

The strategy learnt must get the agent am minimum average score of +13 over 100 consecutive episodes.

### Dependencies & Environment Setup
1. install python 3.6
1. [Clone the DRLND Repository!](https://github.com/udacity/deep-reinforcement-learning#dependencies) and follow the README.md instructions to install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.
1. Download the _ready-built_ Unity Environment:
     1. [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
     2. [Windows 64](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
     3.[Mac](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
1. Place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file

### Use the code
The code has two parts:
1. The **Training phase** {sections 1 - 6} where the agent learns the strategy and saves the resulting model:
  You can try to improve the resulting agent performance working on one of the following:
  1. Changing the hyperparameters in _section 3_ like the discount factor, the soft update parameter or the learning rate
  2. changing the agent nn model structure in _section 4, class QNetwork_ by adding additional layers for example
2. The **Game phase** {section 7} where the saved agent model is loaded and used to play the environment and the score is displayed:
  Here the agent plays a single game and the resulting score is displayed at the end of the game.
