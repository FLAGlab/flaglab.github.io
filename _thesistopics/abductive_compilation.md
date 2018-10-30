---
title: Abductive Debuggers for Program (self) Explanation
period: 2019
level: master
area: pil
abstract: Debuggers provide localized information whenever an error is detected in the system. However, such information provides little to no information explaining the cause of the error. This thesis aims to implement a debugger that explains the resons why code braeks and helps you to solve them.
people: Nicolas Cardozo
---

### Context
Testing is a crucial step in the software development process. In the early stageas of development, developers usually try out their programs by running them locally with specific inputs. This interaction usually leads to discovering bugs in the application. For example, due to arithmetic errors or null pointers. In such cases the error handling method of the system takes over, raising an exeception.

Most of the times, exceptions raised by the runtime system are none-descriptive. As a consequence, developers have little to no information to solve the problems raised by the system, or the reasosns why they arose.

### Project proposal
The main objective of this project is to implement a new debugger equipped with an abductive reasoner [1] to enable the to backtrace the cause of errors found in the program (i.e., execptions) to provide more information to developers.



### Implementation plan
To implement the abductive debugger, we will use the Smalltalk language [2]. This decision is driven by the fully reflective system (e.g., Java reflaction) available in the language. Additionally we will use couple the debugger to with the __lively programming__ programming technique of Smalltalk, in which programs do not crash, but rather are paused, can be fix and continue without errors.


### Background and Literature
[1] Abductive reasoning
[2] PharoSmalltalk
[3] Abduction in Smalltalk
[4] Debugger implementation