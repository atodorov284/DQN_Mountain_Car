# DQN_Mountain_Car
This notebook implements a DQN for the mountain car environment.

The mountain car environment is notorious as it initially requires huge exploration. I made a custom reward function based on velocity, success (finishing an episode before timesteps run out), and a punishment for taking too long. The network is only 3 linear layers with 24 neurons each and ReLU activations.

The agent learns to accelerate by going left and then right, allowing it to complete the episode faster, thus granting the success reward and less punishment for taking too long.
