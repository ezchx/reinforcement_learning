# reinforcement_learning

__(1) very_simple_rl.ipynb__    
- Simple example of Q-learning
- Agent moves left or right until it discovers the treasure (T) at the far right
- Discrete actions and finite # of states

Based on: https://github.com/MorvanZhou/Reinforcement-learning-with-tensorflow/blob/master/contents/1_command_line_reinforcement_learning/treasure_on_right.py    
Q-Learning: https://en.wikipedia.org/wiki/Q-learning    

<img src="https://github.com/ezchx/reinforcement_learning/blob/master/cartpole.gif">

__(2) cartpole_simple_dqn.ipynb__    
- Based on (1) above with infinite states - i.e. Q-table is a neural network
- Simulations are saved in a memory object, randomly sampled as a batch, and used to train the neural network
- Epsilon decays every episode to reduce variability as the network trains
- Achieves a reward of 200 at 120 episodes

Based on: https://github.com/udacity/deep-learning/blob/master/reinforcement/Q-learning-cart.ipynb    
and: https://gist.github.com/tsu-nera/edd306ddeefebe4afb1efceefbc3f953    
Open AI gym: https://gym.openai.com/    

__(3) mountain_car_simple_dqn.ipynb__
- Based on (2) above with mountain car environment and parameters
- Note the two environments:
    - env = gym.make("MountainCar-v0") # capped at 200 moves
    - env = gym.make("MountainCar-v0").env # unlimited moves
- Note the high learning rate (0.5) and low exploration rate (0.1)
- Solves in 20 episodes for the capped environment
- Solves in 3 episodes for the unlimited environment
