### Elastic Weight Consolidation
* Preserve weights according to importance to previous task(s)
* Papers:
  * [Enabling Continual Learning in Neural Networks](https://deepmind.com/blog/enabling-continual-learning-in-neural-networks/)

### Progressive nets
* Papers:
  * [Sim-to-Real Robot Learning from Pixels to Progressive Nets](https://arxiv.org/pdf/1610.04286v1.pdf)
  * [PathNet](https://arxiv.org/pdf/1701.08734.pdf)

### Policy Distillation
* Idea: Transferring knowledge of multiple reinforcement learning policies into a single multi-task policy
* Vanilla policy distillation: transfer policies learned from multiple teacher networks to one student network via supervised regression (state, q-value pairs).
* Training student Q-network by matching the output distributions between student/teacher Q-networks using KL-divergence is more effective.
* Hierarchical Experience Replay: Directly combine layers from the teacher networks to the multi-task policy network + new sampling approach for ER
* Papers:
  * [Knowledge Transfer for Deep Reinforcement Learning with Hierarchical Experience Replay](http://www.ntu.edu.sg/home/sinnopan/publications/[AAAI17]Knowledge%20Transfer%20for%20Deep%20Reinforcement%20Learning%20with%20Hierarchical%20Experience%20Replay.pdf)
  * [Actor-Mimic: Deep Multitask and Transfer Reinforcement Learning](https://arxiv.org/abs/1511.06342)
  * [Policy distillation](https://arxiv.org/pdf/1511.06295v2.pdf)

### Other

[Transfer from Simulation to Real World through Learning Deep Inverse Dynamics Model](https://arxiv.org/pdf/1610.03518v1.pdf)

[Learning and Transfer of Modulated Locomotor Controllers](https://arxiv.org/pdf/1610.05182.pdf)

[learning to do laps with reinforcement learning and neural nets](http://matpalm.com/blog/drivebot/)
