---
title: Python testing
period: 2020
level: undergrad
area: pil
abstract: Implementing a python testing framework
people: Nicolas Cardozo
file: pyunit
---

### Context

Testing pograms is key in the delivery and maintenance processes of software development. Tests are required to assure the implemented functionality behaves correctly. Unit testing, is one of the mos popular testing techniques. However, such technique is not always sufficient for particular parts of a given program.

### Project proposal

In this project we are going to implement a testing framework for Python programs [4] that takes into account two different (independent) aspects.
 1.  First, we want to express success or failure of test cases using First-order assertions. That is, introducing assertions that can quantify over ranges or sets. Te idea behind such assertions is to test system invariants (as they are defined), to bridge the gap between function and data structures definition, their implementation, and their validation.
 2. Second, we want to be able to test different method implementations of a particular behavior seemlessly to the programmer. That is, we want to be able to use exactly the same test cases with different implementations, with no modification to the test-cases. In other words,a unit testing framework that decouples tests from behavior implementation/representation


### Implementation plan

To implement the testing frameqork we will be using Python 3 [1]. In the particular case of the second extension, we will use a Context-oriented programming[2] extention to python, PyContext [3]

### Background and Literature

- [1] [Python](https://www.rust-lang.org)
- [2] Context-oriented Programming: https://www.sciencedirect.com/science/article/pii/S016412121200074X
- [3] PyContext: http://scg.unibe.ch/archive/papers/Loew07aPyContext.pdf
- [4] [PyUnit](https://wiki.python.org/moin/PyUnit)

### Contact
n.cardozo