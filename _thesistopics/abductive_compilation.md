---
title: Abductive Debuggers for Program (self) Explanation
period: 2020
level: master
area: pil
abstract: Debuggers provide localized information whenever an error is detected in the system. However, such information provides little to no information explaining the cause of the error. This thesis aims to implement a debugger that explains the resons why code braeks and helps you to solve them.
people: Nicolas Cardozo
file: abductive_compilation
---

### Context
In modern microservices applications it is hard to replicate and debug issues, because they need to rely on basic logging of each of its parts to diagnose an issue. We will develop novel techniques to automatically reason about the system to provide more descriptive logging information by augmenting it with additional context and high-level information to facilitate debugging and issue resolution.

Today’s software systems are built from various parts, often spanning multiple programs that communicate remotely with each other forming microservice architectures. Such architectures have many benefits for scalability and decoupling. However, they also increase the complexity of the system. For example, when using asynchronous messages to communicate between two microservices, if an error occurs, it becomes more difficult to pinpoint the cause of the error as none of the microservices have complete information about the computation.

The diagnosis and error analysis in such systems relies on log entries produced by the system’s parts which may include log entries about requests processed, and possibly information on exceptions. Unfortunately, log entries and exceptions rarely provide enough context and are not descriptive enough to enable developers to build a regression test and resolve the bug. Instead, developers have to try to reconstruct the circumstances in a testing environment and hope they are able to trigger the bug.
This partial view on these systems makes bug diagnosis hard. While one could simply provide more and more information with additional log entries, this is problematic from a performance and engineering perspective. Furthermore, it would only shift the problem to finding the needle in the haystack.


### Project proposal
The objective of this project is to develop techniques based on abductive reasoning that automatically analyze available run time and log information and provide a higher-level explanation of, for instance, the reason for an exception. This will simplify reproduction and error diagnosis, therefore reducing the cost of bug fixes.

Specifically, abductive reasoning will enable us to utilize contextual information of an error and infer possible causes across microservices by combining the information fragments available from logging as well as the runtime state at the point in which the exception is detected. In a first step, we will instrument a dynamic language runtime such as TruffleRuby to be able to access runtime state on errors as well as to identify which program statements correspond to specific log entries. Then, we will apply abductive reasoning to utilize the information to identify the root-cause of a fault. For this research, we have access to the Ruby source code and issue tracking system of our industrial partners, which allows us to work with real bugs to develop novel abductive reasoning techniques.


### Implementation plan
For this purpose, we rely on previous work on diagnosis and correction of inconsistencies between source code and documentation rules [1], which demonstrates the use of abductive reasoning to detect and correct inconsistencies in source code. Additionally, the use of abductive reasoning has also proven beneficial in dynamic software updates [3] using a process similar to that of abductive reasoning. We will also utilize our previous work on low-overhead tracing [2] and dynamic runtime systems as foundation. This will be especially relevant for an application in microservice environments and its use in production systems.

The project will be implemented in Ruby, and it'll be validated using an industrial case study.


### Background and Literature
 - [1] [Abduction in Smalltalk](https://released.info.ucl.ac.be/pmwiki/uploads/Publications/DiagnosingAndCorrectingDesignInconsistenciesInSourceCodeWithLogicalAbduction/2010-scico-castro.pdf)
 - [2] [Finding Broken Promises in Asynchronous JavaScript Programs](http://ece.ubc.ca/~saba/dl/promisekeeper.pdf)
 - [3] [Automating Object Transformations for Dynamic Software Updating via Online Execution Synthesis](https://cs.nju.edu.cn/changxu/1_publications/ECOOP18.pdf)
 - [4] [Debugger implementation](http://www.sigops.org/s/conferences/sosp/2009/papers/glerum-sosp09.pdf)
 - [5] [Abductive reasoning](https://en.wikipedia.org/wiki/Abductive_reasoning) 


### Contact
n.cardozo