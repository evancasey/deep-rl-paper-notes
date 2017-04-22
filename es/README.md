### Evolutionary Strategy
* Works because reward signal is super weak and ES is highly parallelizable
* Doesn't work when reward signal is strong: training a simple MNIST classification network using ES is “1000 times slower.”
* Not the end-all-be-all: better training methods still need the gradient (eg. predicting the future state of the environment)
* Papers:
  * [Evolution Strategies as a Scalable Alternative to Reinforcement Learning](https://arxiv.org/abs/1703.03864)
* Blog posts:
  * https://blog.openai.com/evolution-strategies/
  * https://chatbotslife.com/reinforcement-learning-or-evolutionary-strategies-nature-has-a-solution-both-8bc80db539b3
