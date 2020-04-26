# Implementation description

</br>

## Learning Algorithm

DDPG agent algorithm with simple replay buffer is used in this project. 
For multi agent version please check [ddpg_multiagent.py](ddpg_multiagent.py) and for single-agent version -  [ddpg_agent.py](ddpg_agent.py).


Configuration for multiagent solution:
* 2 hidden layers with 512 and 300 hidden units for both actor and critic
* Replay batch size 512
* Buffer size 1e6
* Replay without prioritization
* Update frequency 4
* TAU from  1e-3
* GAMMA is 0.99
* Learning rate 1e-4 for actor and 3e-4 for critic
* Noise
I 

</br>

## Plot of Rewards
Plot of rewards can be seen after the environment has been solved. 
You can check the notebook which used for all the work related to multiagent solution [Crawler.ipynb](Crawler.ipynb).

Environment solved in 117 episodes

</br>

## Ideas for Future Work
Here's a list of optimizations that can be applied to the project:
1. Build an agent that finds the best hyperparameters for an agent
2. Prioritization for replay buffer
3. Paramter space noise for better exploration
4. Test shared network between agents
5. Test separate replay buffer for agents
6. Implement dedicated D4PG or PPO algorithms to improve general performance
