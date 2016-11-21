Third Person Imitation Learning
-------------------------------

# Source

Paper: https://openreview.net/pdf?id=B16dGcqlx
Code: https://github.com/bstadie/third_person_im

# Prerequisites

1. Generative Adverserial Imitation Learning

See: http://github.com/evancasey/paper-notes/generative-adverserial-imitation-learning.md

# The basic idea

Recall that the initial layers in a CNN contain domain specific feature representations. Thus, there is mutual information contained in the domain label (expert vs novice domain) and the feature layers of the discriminator function.

The goal is to enable the non-expert policy to act in a different environment with out allowing the discriminator function to learn these differences (since it would use them as a strong classification signal and that would screw things up). 

The paper solves this by adding another optimization objective which is to maximize domain confusion - the probability that features produced by the discriminator were produced by the expert vs non-expert environment.

# Results 

[TODO]
