Generative Adverserial Imitation Learning
-----------------------------------------

# Source

Paper: https://arxiv.org/pdf/1606.03476v1.pdf

# Prerequisites

1. Inverse Reinforcement Learning

Recall that the reward function takes state --> reward. We try to recover the reward function by taking a bunch of trajectories from an expert policy and find a cost function under which the expert is uniquely optimal.

Why learn cost function when what we really want to learn is the policy?

2. Apprenticeship Learning

[TODO]

# The basic idea

We simultaneously train $\pi_\theta$ (the policy we're trying to learn, which is initialized randomly) and $D_{w}(s)$ (the discriminator function). $D_{w}(s)$ outputs the probability of a state having originated from a trace from the imitator policy.

$\pi_\theta$ and $D_w$ are trained adverserially. That is, we're trying to find a policy that makes it impossible for a discriminator to distinguish states visited by the expert from states visited by the imitator agent.

# Results 

[TODO]


