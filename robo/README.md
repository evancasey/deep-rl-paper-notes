### Surveys
* CNNs overgeneralize:
  * can be more robust if you give it more than just RGB images (depth, tactile information with physical adversarial entities)
  * pixel level segmentation + object detection need for rule-based navigation —> how to connect this to motor control?

* GPS
   * Used heuristic for classifying grasp examples

* Most game playing deep RL is on fully observable environments
  * most real world applications are partially observable
  * transfer from sim to real often requires massaging the scene to mimic the simulation setting
  * progressive nets pose one possible solution but assumes known task boundaries and exhibits quadratic parameter growth when a new column is necessary for each novel domain. results on real world were still highly constrained
  * work being done for domain alignment by Tzeng et al (Towards adapting deep visuomotor representations from simulated to real environments), but this requires paired synthetic and real views of the same scene to adapt the deep visual representations.

* Ultimately, robots must collect their own training data in the real world (self-supervision)
  * Current work doesn’t address continual learning, need framework for robots to collect and label examples themselves
  * Proposed solution: hierarchical set of motor behaviors + intrinsic motivation (information theoretic measures)


* Papers:
  * [Deep reinforcement learning for robotic manipulation-the state of the art](https://arxiv.org/pdf/1701.08878v1.pdf)
  * [Deep-learning in Mobile Robotics - from Perception to Control Systems: A Survey on Why and Why not](https://arxiv.org/pdf/1612.07139.pdf)
  * [Towards Lifelong Self-Supervision:A Deep Learning Direction for Robotics](https://arxiv.org/pdf/1611.00201v1.pdf)

### Self-driving cars
* Papers:
  * [End to End Learning for Self-Driving Cars](https://arxiv.org/pdf/1604.07316.pdf)
* Lectures:
  * [Deep Learning for Self-Driving Cars](https://www.youtube.com/watch?v=nFTQ7kHQWtc)

### Drones
* Papers:
  * [A Machine Learning Approach to Visual Perception of Forest Trails for Mobile Robots](http://rpg.ifi.uzh.ch/docs/RAL16_Giusti.pdf)
  * [Uncertainty-Aware Reinforcement Learning for Collision Avoidance](https://arxiv.org/pdf/1702.01182v1.pdf)
  * [CAD^2RL](https://arxiv.org/pdf/1611.04201.pdf)
  * [Learning Deep Control Policies for Autonomous Aerial Vehicles with MPC-Guided Policy Search](http://rll.berkeley.edu/icra2016mpcgps/ICRA16_MPCGPS)
