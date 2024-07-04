---
title: Evaluation of Transfer Learning Techniques for Multi-task environments in Robot systems.
period: 2024
level: master
area: ai
abstract: Evaluation of transfer learning algorithms to enable robot behavior in different unknown scenarios (unknown actions, unknown rewards)
people: Nicolás Cardozo
file: transferlearning-unknown
layout: default
---

### Context

Reinforcement Learning (RL) and in particular Deep Reinforcement Learning (DeepRL) are popular learning techniques to adapt the behavior of agents. Through the interaction with the environment, agents learn the best set of actions for the different observed states. Over time, the agents specialize their behavior to a given set of actions, exploiting the optimized learned actions. According to the environment size, learning of optimal actions may take a long time. Morover, if the environment changes, learned actions may become unusable or just wrong, leading to a long learning process again.

### Project proposal

The purpose of this project is to evaluate transfer learning algorithm, that enable the sharing of learned information (i.e., states and action) between agents as a means to accelerate learning and to deal with unknown situations or environments.

### Implementation plan

The evaluation of transfer learning algorithms will start with their implementation (different variants), and the implementation of a DQN base agent (to be used as baseline). The agents will be trained on a standard environment (e.g., melting pot environment) and test for performance. Then, the agents will move into different scenarios to evaluate their performance. Finally, we will take advantage of transfer information to improve agent behavior in an environment and across environments.

### Contact

n.cardozo
