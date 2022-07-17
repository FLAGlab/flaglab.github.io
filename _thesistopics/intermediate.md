---
title: Intermediate language for airplane systems
period: 2022
level: undergrad
area: pil
abstract: Implement an intemediate language to reason about airplane programs
people: Nicolas Cardozo
file: intermediate
---

### Context

Like must modern systems, airplanes are managed by software. Normally, software in big systems deals with a large amount of variability in its specification and implementation. In particulary, the many components composign the original system might be implemented using different programming techniques and languages. While each individual component is rigorously tested (as airplanes are safety critical systems), testing the system as a whole is more challenging, due to the language barriers.

### Project proposal

In this project, we want to explore the different programming language in which airplane components are developed, and propose an intermediate language, common to all. The objective of the language is offer a clean simple core in which different safety properties can be verified.

### Implementation plan

- Literature review on programming language for airplane components
- Develop a reduce intermediate language for verification.
- Implement compilers for the different languages to the proposed intermediate language
- Validate the compilation problem, proving equivalence of programs

### Background and Literature

- Language definition
- Compiler construction

### Contact

n.cardozo
