### Guided Policy Search
* GPS learns an end-to-end motor control policy from raw pixel input that is more sample efficient than other more popular deep RL approaches (think DQNs or PGs). To do this, GPS first learns a guiding distribution p_i(u_t|x_t) using the full state of the system (joint angles and velocities) via trajectory optimization. This guiding distribution is conditioned on some initial state and is easier to optimize via optimal control methods (i.e. LQG) since it can use the full state of the system.
* Using the trajectory distribution p(\tau) generated from the guiding distription, a policy \pi_\theta(u_t|x_t) is optimized to match p(\tau). The samples generated from this rollout are also used to optimized each p(\tau), since we need the policy and guiding distribution to be generated from the same state distribution.
* This optimization method of alternating between trajectory-centric RL and supervised is formalized as a variant of the BADMM algorithm (Wang and Banerjee, 2014) for constrained optimization, which can be used to show that, at convergence, the policy and the guiding distributions will exhibit the same behavior.
* To speed up learning, the vision layers in the policy and the trajectory distributions for guided policy search are initialized by pose regression CNN. The robot moves the target object through a range of random positions, recording camera images and the object’s pose, which is computed automatically from the pose of the gripper.
* Papers:
  * [Guided Policy Search](https://graphics.stanford.edu/projects/gpspaper/gps_full.pdf)
  * [Learning Contact-Rich Manipulation Skills with Guided Policy Search](http://rll.berkeley.edu/icra2015gps/robotgps.pdf)
  * [End-to-End Training of Deep Visuomotor Policies](https://arxiv.org/pdf/1504.00702v5.pdf)
  * [Guided Policy Search as Approximate Mirror Descent](https://arxiv.org/pdf/1607.04614v1.pdf)

### Distributed Guided Policy Search 
* Papers: [Collective Robot Reinforcement Learning with Distributed Asynchronous Guided Policy Search](https://arxiv.org/pdf/1610.00673.pdf)

### Value Iteration Networks
* Papers: [Value Iteration Networks](https://arxiv.org/pdf/1602.02867v2.pdf)
