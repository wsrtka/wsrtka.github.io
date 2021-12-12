---
layout: default
permalink: /concepts/types-of-learning
---

# Types of learning

## Supervised learning
A supervised machine-learning system is one that needs labeled data to develop a useful understanding. This is called its model. If it's output is descrete with few values, it is called a classifier. If it can result in many values, which have a natural ordering, it is called a regressor. The essence of a supervised machine-learning algorithm is to figure out the parameters of a model that result in the least cost.

## Unsupervised learning
Unsupervised learning is about modeling data that comes without corresponding labels or responses. Some examples include: clustering, PCA.

## Reinforcement learning
A branch of machine-learning, in which the environment acts as a teacher, providing hints as opposed to definite answers. The learning system receives feedback on its actions, with no concrete promise that is is in fact progressing in the right direction. It trains on information gathered by observing how the environment reacts to actions. An important concept here is the struggle of exploration vs. exploitation - deciding when the model should experiment and search for new, potentially better actions as opposed to exploiting the decisions which were found best until now.

The system is typically refered to as an autonomous agent. The status of the world frozen at a particular time is called a state. An agent may perform one of many actions to change the current state. To drive an agent to perform actions, each state yields a corresponding reward. An agent eventually discovers the expected total reward of each statem cakked the value of a state.

## Meta-learning
An area of machine-learning searching to automate the process of selecting, training, deploying, optimizing and evaluating models.
