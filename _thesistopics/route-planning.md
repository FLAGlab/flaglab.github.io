---
title: Dynamic Planning for Navigation Routes in Unknown Environments
period: 2022
level: undergrad
area: algo
abstract: Using dynamic planning and execution techniques to design the navigation routes of self-driving robots in unknown situations
people: Nicolás Cardozo
file: route-planning
---

### Context

Self-driving robots have to fulfill many different operations, as the coordination of mechanics in the robot (e.g., traction of motors, camera movement, actuator arms), and the actual movement of the robots --that is, driving to the places they need to reach.

This task is the outmust importance for exploration robots, which must  drive around exploring an area in an unknown terrain. As the area to drive is unknown, planing a specific route and driving plan is challenging, given that the chosen plan could be inapropriate for the given terrain, or even may find a mission with varying environments, which may not be appropriate for a given plan.

### Project proposal

In this project we are going to explore dynamic navigation planning techniques so that when the driving environment changes, the robot can have a driving plan that is the most appropriate for each specific environment.

To reach this goal, we will first explore different driving plan algorithms evaluating their characteristics; in particular the conditions for optimality. Having this, we can explore different dynamic execution techniques to be able to modify the navigation plan and mantain optimal performance.

### Implementation plan

- Literature review about driving plan algorithms
- Implement evaluation scenarios for the different algorithms
- Implement dynamic adaptation plans for algorithms in robot environments
- Evaluate the dynamic algorithm in different scenarios compared with the initial evaluation.

### Background and Literature

- Context-oriented programming
- ROS

### Contact

n.cardozo
