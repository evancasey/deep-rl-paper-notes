Prioritized Experience Replay
-----------------------------

# Source

Paper: https://arxiv.org/abs/1511.05952

# The basic idea

In Vanilla DQN, we store transitions in a bounded experience replay buffer. At each rollout, we compute the gradient update from a randomly sampled mini batch of examples from this buffer. This is to get rid of “feedback loops”, since exploring a certain portion of the environment will yield examples from this portion.

In prioritized experience replay, we weight the examples in the experience replay buffer by TD-error, which measures how surprising the transition was.
