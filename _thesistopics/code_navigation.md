---
title: Kotlin plug-in for code navigation
period: 2022
level: undergrad, master
area: pil
abstract: 
people: Nicolas Cardozo
file: code_navigation
---

### Context

Developers usually spend must of their time debugging code, which obviously makes for not very productive developers. New tools and debugging techniques are all amied at easing the debugging process for developers.

This is particularly true for complex applicactions (e.g., concurrent or asynchronous environmentments) in which debugging a program is particularly difficult, as the states are not always reproducible or easy to reach. To counter these problems, a new type of debuggers, called back-in-time [1,2] debuggers was created. These debuggers, have the ability to not only step into and over instructions, but also to step back from an instruction. That is, we can revert the state of a program to the state before executing a given instruction.  

### Project proposal

In this project we want to explore the development of such a debugger for the Kotlin programming language [3]. Kotlin programs have the characteristics to run concurrent, asynchronous programs that can benefit from back in time debugging techniques. The debugger should run as a plugin for the Kotlin IDE, IntelliJ.

### Implementation plan

To build a back-in-time debugger, one of the available techniques is to use continuations [4]. Continuations let you capture the state of a program at any point in the computation, which then can be restored at anyother point. This technique can be used to define explicit and implicit time points [5], to which the system can go back to. In fact, part of the implementation plan, is to replicate the model of Delorean [5] applied in the context of Kotlin.

The second part of the implementation plan is to explore different graphical interfaces to ease the navigation of code throught the execution time. In particular, the tool will allow developers to the specify variables/functions in the program to record their change history, to observer the evolutions of its values.

### Background and Literature

[1] [Omniscient Debugging](https://ieeexplore.ieee.org/abstract/document/5287015)
[2] [Object-oriented Back-in-time debugging](https://link.springer.com/chapter/10.1007/978-3-540-70592-5_25)
[3] [kotlin](https://kotlinlang.org)
[4] [Continuations](http://www.math.bas.bg/~bantchev/place/iswim/conti-disco.pdf)
[5] [DeloreanJS](https://youtu.be/bGZ73Dtpt6E)

### Contact

n.cardozo
