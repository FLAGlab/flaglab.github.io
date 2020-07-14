---
title: Game theoretic work stealing
period: 2020 
level: undergrad
area: pil
abstract: Applying game theory strategies to optimize work-stealing algorithms
people: 
file: 
---

### Context

Work stealing [1] is a common technique sused in prallel computing to take advantage of node or processes that are idle. Whenever a process becomes idle, because it has finished its work, rather than waiting for other processes to finish, it can reduce teh wait time by taking up some of the tasks assign to other processes. The overall objective of this technique is to speed-up program execution. Taking into account this objective, game theory strategies [2] could be applied as a work-stealing technique, in which the overall behavior of the system is guaranteed by the stealing decisions taken by processors.

### Project proposal

This prject will explore game theory strategies that maximize the well being for all processes (in terms of their idle and active times) as a means to speed-up parallel computation. In this project we will explore different application domains in which the proposed work-stealing techniques are beneficial.

### Implementation plan

The project will be based in the exploration of different game thepry strategies applied to well known work-stealing data sets [3].

### Background and Literature

[1] Scheduling multithreaded computations by work stealing<https://dl.acm.org/doi/abs/10.1145/324133.324234>
[2] Multiagent Systems <http://www.masfoundations.org/mas.pdf>
[3] An Empirical Evaluation of Work Stealing with Parallelism Feedback <http://people.csail.mit.edu/kunal/adapt-exp.pdf>

### Contact

n.cardozo
