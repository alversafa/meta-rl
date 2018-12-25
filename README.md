# Meta Reinforcement Learning

Simple implementation of meta reinforcement learning experiments in PyTorch.

**Dependencies:** pytorch 0.4, numpy, matplotlib

Experiments:

* [depbandit_1.ipynb](depbandit_1.ipynb): Dependent bandit experiment I from the 
[Learning to reinforcement learn](https://arxiv.org/abs/1611.05763) paper by
J. Wang et. al

	In this experiment, the agent is trained on a distribution of dependent 2-armed
	bandits and it is asked to solve particular 2-armed bandits where the reward giving
	arm is changed in each test episode.

* [depbandit_2.ipynb](depbandit_2.ipynb): Dependent bandit experiment II from the 
[Learning to reinforcement learn](https://arxiv.org/abs/1611.05763) paper by
J. Wang et. al

	In this experiment, the agent is trained on a distribution of dependent 11-armed
	bandits with deterministic payouts. The nine non-target arms give a reward of 1,
	the one target arm gives a reward of 5, and the eleventh arm gives an informative
	reward (<1) of one tenth the target arm's index as 0.2 when the target arm is 2.
	It is expected from the agent to pay a short-term reward cost to gain information
	on the target arm and keep pulling it.