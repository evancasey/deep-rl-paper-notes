
### REINFORCE
* Introduces the REINFORCE policy gradient algorithm, which directly learns a parameterized policy using error back-propagation.
* Used to solve a variety of simple, low-dimensional discrete and continuous control tasks.
* Papers:
  * [Policy Gradient Methods for Reinforcement Learning with Function Approximation](https://webdocs.cs.ualberta.ca/~sutton/papers/SMSM-NIPS99.pdf)
  * [Reinforcement learning of motor skills with policy gradients](http://www.keck.ucsf.edu/~houde/sensorimotor_jc/possible_papers/JPeters08a.pdf)
* Blog posts:
  * http://www.rage.net/~greg/2016-07-05-ActorCritic-with-OpenAI-Gym.html

### Deep Deterministic Policy Gradients (DDPG)
* Like REINFORCE, DDPG directly learns a parameterized policy in addition to a value function. However, unlike the stochastic policy gradient, it uses a deterministic policy gradient
* Applied to ALE and Mujoco tasks
* Papers:
  * [DDPG](http://jmlr.org/proceedings/papers/v32/silver14.pdf)
  * Continuous control
* Blog posts:
  * https://papers.nips.cc/paper/5796-learning-continuous-control-policies-by-stochastic-value-gradients.pdf
  * http://pemami4911.github.io/blog_posts/2016/08/21/ddpg-rl.html
  * https://yanpanlau.github.io/2016/10/11/Torcs-Keras.html
  * http://techtalks.tv/talks/deterministic-policy-gradient-algorithms/61098/

### Trust-region Policy Optimization (TRPO)
* Prevents the policy gradient updates from exceeding a KL-divergence bound. Improves learning stability and hyperparameter sensitivity
* Applied to ALE and Mujoco tasks, outperforms DDPG on many continuous control Mujoco tasks
* Papers: 
  * [TRPO](https://arxiv.org/abs/1502.05477)
* Blog posts:
  * Kv frans
* Other
  * https://github.com/openai/requests-for-research/pull/22#issuecomment-250386140

### High-dimensional continuous control using generalized advantage estimation
* Introduces theoretical framework that shows that advantage params determine bias-variance trade-off

### Asynchronous Advantage Actor-Critic
* Papers:
  * [A3C](https://arxiv.org/abs/1602.01783)
* Blog posts:
  * http://www.allinea.com/blog/201607/tuning-deep-learning-episode-1-deepminds-a3c-torch
  * https://github.com/Kaixhin/Atari/issues/5
  * https://github.com/kuz/DeepMind-Atari-Deep-Q-Learner
  * https://medium.com/emergent-future/simple-reinforcement-learning-with-tensorflow-part-8-asynchronous-actor-critic-agents-a3c-c88f72a5e9f2#.gtkdbo3a
  * https://jerrybai1995.github.io/2016-11-30-doom-ai/

### ACER
* Papers:
  * [ACER](https://arxiv.org/pdf/1611.01224.pdf)

