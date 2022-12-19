---
title: Fast Fast Bayes Library
period: 2023
level: undergrad
area: algo
abstract: While python is very popular for ML development, it is also very slow to fulfill such purpose. We need to implement popular network libraries in faster languages.
people: Nicolas Cardozo, Mario Linares
file: fast_bayes
---

### Context

Bayesian networks is an important probabilisitc model that has become ever more popular with the explosion of Machine Learning algorithms and applications. For this reason, many libraries have been implemented in Python, a programming language popular for the development of ML solutions. However, among the programming languages community, Python is known to be a slow language, defeating the purpose of its use for heavy weight processing as in the case of ML.

### Project proposal

In this project we will explore the performance of Python ML libraries, in contrast to new implementations in other (faster?) languages, like Rust [1], Carbon [2], or C++. In particular we will explore the performance of the PyBNesian [3] library for processing bayesian networks.

### Implementation plan

To satisfy our objective, we will start by defining a set of performaance benchmarks for the PyBbNesian library, but general to other ML libraries.
Following this, we will reimplement the library using languages known for their performance, like Rust, Carbon, and C++. This, to have a comparative performance evaluation of the library.

### Background and Literature

Knowledge about algorithms' performance is rerquired for this thesis, additional information about the languagees to use is available at:

- [1] <http://rust-lang.org>
- [2] <https://github.com/carbon-language/carbon-lang>
- [3] <https://readthedocs.org/projects/pybnesian/>

### Contact

n.cardozo
m.linarev
