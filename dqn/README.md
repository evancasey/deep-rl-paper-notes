### Deep Q-Networks
* Introduces DQNs for control from raw-pixel inputs, which uses Bellman updates to learn an action-value function and off-policy action selection using the learned action-value function. Demonstrates how experience replay helps the algorithm get an even distribution of experience (eg. avoid "feeback loops").
* Learns to play a large number of Atari games. However, the algorithm is extremely sample inefficient.
* Papers:
  * [Playing Atari with Deep Reinforcement Learning (DQN)](https://arxiv.org/pdf/1312.5602v1.pdf)
  * [Beating the World's Best at Super Smash Bros. with Deep Reinforcement Learning](https://arxiv.org/abs/1702.06230)
* Blog posts:
  * http://neuro.cs.ut.ee/demystifying-deep-reinforcement-learning/
  * https://rubenfiszel.github.io/posts/rl4j/2016-08-24-Reinforcement-Learning-and-DQN.html
  * https://medium.com/@awjuliani
  * https://devblogs.nvidia.com/parallelforall/deep-learning-nutshell-reinforcement-learning/
  * https://vmayoral.github.io/robots,/ai,/deep/learning,/rl,/reinforcement/learning/2016/08/07/deep-convolutional-q-learning/

### Prioritized experience replay
* Introduces prioritized experience replay, an improved version of the experience replay strategy used in the DQN paper. In prioritized experince replay, examples in the experience replay buffer are weighted by TD-error, which measures how surprising the transition was.
* Shows improved performance on ALE.
* Papers:
  * [Prioritized experience replay](https://arxiv.org/pdf/1511.05952v4.pdf)

### One step q-learning
* Papers:
  * [One step q-learning](http://jmlr.org/proceedings/papers/v32/silver14.pdf)

### Dueling DQN
* Papers:
  * [Dueling DQN](https://arxiv.org/abs/1511.06581)
* Other:
  * https://m.reddit.com/r/MachineLearning/comments/57ec9z/discussion_is_my_understanding_of_double/?utm_source=mweb_redirect&utm_medium=twitter&compact=true

### Continuous Deep Q-Learning with Model-based Acceleration (NAF)
* Continuous version of DQN that efficiently computes argmax(Q).
* Papers
  * [NAF](https://arxiv.org/pdf/1603.00748.pdf)

### Q-Prop
* Papers:
  * [Q-Prop](https://arxiv.org/abs/1611.02247)

### Reactor
* Papers:
  * [The Reactor: A Sample-Efficient Actor-Critic Architecture](https://arxiv.org/pdf/1704.04651.pdf)
