---
title: Consistency verification of COP programs using session types
period: 2024
level: master
area: pil
abstract: Type systems are used to assure behavior of a system. This project will tackle the consistency and interaction of dynamic behavior for adaptive systems
people: Nicolas Cardozo
file: session-cop
layout: default
---

### Context

The high interaction of software systems requieres them adapt to their surrounding execution context. One technique to cope with this requirement is achieved, at the programming langauge level, using Context-oriented programming (COP) [2]. With the advancements of COP, it is possible to develop modular programs that can change their behavior in response to changes in the surrounding environment, or context.

However, the dynamic modification of a program's behavior opens up the possibility of bugs during the execution of a program, due to inconsistencies or incompatibilities of the introduced behavior. This problem increases in the precence of multiple interacting contexts.

### Project proposal

The effect of bugs or inconsistent behavior in the execution of COP programs is a symptom of the lack of assurances present in the system, as no verification can take place on-line due to time complexity of such processes.

In this project we aim to use session types [1] as a verification mechanims to assure the absense of inconsistencies of interacting contextual behavior. The use of session types in this context is of particular interest in this context, as session types are used to express interactions between entities, in our case, the interactions between the adapted behavior definitions.

### Implementation plan

The implementation plan of this thesis is as follows.

- Development of session types into a COP programming language, as ContextScala
- Design of a session type model for COP
- Implementation of the verification behavior to detect inconsistencies in COP programs.

### Background and Literature

- [1] [Session types](https://dl.acm.org/doi/10.1145/2370776.2370794)
- [2] [Context-oriented programming](https://dl.acm.org/doi/10.1145/2451436.2451461)

### Contact

n.cardozo
