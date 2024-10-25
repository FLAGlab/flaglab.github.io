---
title: MCI. Minimal Circular Intersection Algorithm
period: 2023
level: undergrad
area: algorithms
abstract: Visualization is important for the success of informtive software. Setting a correct layout can change the perception of a result from simple to complex. We will improve the visualization of circular layouts.
people: Nicolas Cardozo, Jorge Duitama
file: circular_intersection
layout: default
---

### Context

Data visualization has become quite an important topic in the last couple of years, given the 
increasing interest for data intensive software systems. Offering a good visualization of data
can make the difference in a decision making process, or help to understand and give meaning to the information used/returned in a system.

### Project proposal

A particular visualization often used to demonstrate relations across data points (for example representing system modules or information correlation), is to use a circular representation. However, the way in which the data points are located on the circumference can make the difference between a messy visualization and a clear one.

In this project we are interested in developping a new efficient algorithm that, given a set of points and the relations between them, can place them in a circular layout ensuring the least amount of crossings (i.e., intersections) between the edges connecting the data points.

### Implementation plan

We are interested in developping an efficient algorithm. Therefore, the implementation must include performance data evaluations with different (generated) test cases at different scales.

Additionally, we want to evaluate the algorithm on a real-world application. In this case we will use the information and integrate the algorithm with NGSEP [1], a framework for the analysis of of genome sequences.

### Background and Literature

- [1] NGSEP: <https://sourceforge.net/p/ngsep/wiki/Home/>

### Contact

n.cardozo
