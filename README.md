# reinforcement_learning

__(1) very_simple_rl.ipynb__    
- Simple example of Q-learning
- Agent moves left or right until it discovers the treasure (T) at the far right
- Discrete actions and states

Q-Learning: https://en.wikipedia.org/wiki/Q-learning    
Based on: https://github.com/MorvanZhou/Reinforcement-learning-with-tensorflow/blob/master/contents/1_command_line_reinforcement_learning/treasure_on_right.py    

<img src="https://github.com/ezchx/reinforcement_learning/blob/master/cartpole.gif">

__(2) cartpole_simple_dqn.ipynb__    
- Similar to (1) except with continuous states - i.e. Q-table is a neural network
- Simulations are saved in a memory object, randomly sampled as a batch, and used to train the neural network
- Epsilon decays every episode to reduce variability as the network trains
- Achieves a reward of 200 at 120 episodes

Based on: https://github.com/udacity/deep-learning/blob/master/reinforcement/Q-learning-cart.ipynb    
and: https://gist.github.com/tsu-nera/edd306ddeefebe4afb1efceefbc3f953
