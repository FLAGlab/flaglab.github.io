---
title: Symbolic execution for Type Verification of Python Programs
period: 2022
level: master
area: pil
abstract: Implement a symbolic execution engine that checks the consistency of variable types
people: Nicolas Cardozo
file: symbolic_python
---

### Context

Python is a foreign language for Java and C++ programmers as it is dynamically type. This has two particular implications in python. First, variables do not have to be accompanied by a type declaration. Second, variables can change their type. This has very important implications in terms of program comprehension. 

### Project proposal

The idea of this project is to implement a symbolic execution engine [1] that is able to detect and track types of variables from the first moment they are introduced to the completion of a program. Using this analysis it will be possible to signal developers about misuses of variables or potential type errors that may exist in the program.

### Implementation plan

The engine is to be implemented in Python to integrate easily with the target systems to validate.

### Background and Literature

- [1] Symbolic Execution and Program Testing. King, James C. Commun. ACM. 1976.

### Contact

n.cardozo