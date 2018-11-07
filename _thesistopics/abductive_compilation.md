---
title: Abductive Debuggers for Program (self) Explanation
period: 2019
level: master
area: pil
abstract: Debuggers provide localized information whenever an error is detected in the system. However, such information provides little to no information explaining the cause of the error. This thesis aims to implement a debugger that explains the resons why code braeks and helps you to solve them.
people: Nicolas Cardozo
file: abductive_compilation
---

### Context
Testing is a crucial step in the software development process. In the early stageas of development, developers usually try out their programs by running them locally with specific inputs. This interaction usually leads to discovering bugs in the application. For example, due to arithmetic errors or null pointers. In such cases the error handling method of the system takes over, raising an exeception.

Most of the times, exceptions raised by the runtime system are none-descriptive. As a consequence, developers have little to no information to solve the problems raised by the system, or the reasosns why they arose.

### Project proposal
The main objective of this project is to implement a new debugger equipped with an abductive reasoner [1] to enable the to backtrace the cause of errors found in the program (i.e., execptions) to provide more information to developers.



### Implementation plan
To implement the abductive debugger[3,4], we will use the Smalltalk language [2]. This decision is driven by the fully reflective system (e.g., Java reflaction but well done) available in the language. Additionally we will couple the debugger to with the __lively programming__ programming technique of Smalltalk, in which programs do not crash, but rather are paused, can be fix and continue without errors.


### Background and Literature
[1] [Abductive reasoning](https://en.wikipedia.org/wiki/Abductive_reasoning)

[2] [PharoSmalltalk](https://pharo.org)

[3] [Abduction in Smalltalk](https://released.info.ucl.ac.be/pmwiki/uploads/Publications/DiagnosingAndCorrectingDesignInconsistenciesInSourceCodeWithLogicalAbduction/2010-scico-castro.pdf)

[4] [Debugger implementation](http://www.sigops.org/s/conferences/sosp/2009/papers/glerum-sosp09.pdf)

### Contact
n.cardozo