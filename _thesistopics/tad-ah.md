---
title: TAD-ah
period: 2022
level: master
area: algorithms
abstract: TAD-ah is a new language implementation based on Abstract Data Types (ADTs) that does not have null
people: Nicolas Cardozo
file: tad-ah
---

### Context

One of the biggest issues in object-oriented software development, causing increased development and maintenance costs, are run-time exceptions. The most common exception found in software development is the famous NullPointerException, in which the program trys to access properties or behavior of a de-referenced object (a null pointer), not being able to execute the desired instruction.

Over the last couple of years different proposals to diminish NullPointerExceptions, modern programmin languages as Scala, Swift, or Kotlin introduce nullable objects, which replicate the type system lattice, to provide versions of objects that can never be null. Rust, provides ownership concepts to ensure is not possible to access dereferenced objects.

### Project proposal

In this project we want to take a different approach, building a programming language, TAD-ah, that, from the ground up, does not introduce null values, avoiding NullPointerExceptions altogether.
TAD-ah, will be based on Abstract Data Types (ADTs) [1,2], which will require a base entity as the inception of each type. With TAD-ah we will explore the use of inductive definitions for ADTs and template objects to manage referencing and dereferencing objects in our programs.

### Implementation plan

The idea of the language is to start with a minimal implementation of basic types and objects to start exploring the idea of a purely ADT-based language, and how this can help us avoid NullPointerExceptions 

### Background and Literature

[1] CLU - http://pmg.csail.mit.edu/~dcurtis/clu/
[2] A History of CLU. HOPL-II: The second ACM SIGPLAN conference on History of programming languages 1993. B. Liskov

### Contact

- n.cardozo
