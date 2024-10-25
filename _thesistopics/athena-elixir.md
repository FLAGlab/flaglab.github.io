---
title: Verification and testing, together again for the first time
period: 2025 
level: master
area: pil
abstract: Create a language bridge between a formal verification language (Athena) and programming language (Elixir) to assure the correct execution of distributed systems
people: Mateo Sanabria, Nicolas Cardozo
file: athena-elixir
layout: default
---

### Context

Distributed programming increases the level of complexity of software systems, given the temporal and physical distribution. Communication between program entities becomes a hard problem to solve due to the contunuous disconenction.

The new layer of complexity adds fragility to the system, as assuring properties about its behavior becomes more challenging, or is not done at all. Common validation techniques, as testing are not enough to validate the system behavior, as reproducing bugs and disruptions is difficult. Verification of the system is often not done given that is time consuming, and it requieres to leave the programming environment, often generating a mismatch in the abstraction level.

### Project proposal

In this thesis we are want to develop a language bridge between a distributed programming language, and a verification language (Elixir [2] and Athena [1], respectively), creating a casual connection between them.
The effect of this conenction is that it is now posible to define proofs that are naturally translate to working code and vise-versa.As a consequence, it will be possible to verify the behavior of of distributed programs directly at development time, reducing the verification cost, and completely eliminating the abstraction mismatch between languages

### Implementation plan

The implementation of this project consists of a dual IDE in which is possible:

  1. Write Elixir programs that "renders" to athena verification code.
  2. Write Athena proofs that "renders" Athena code to Elixir

To do this, it is necessary to create a mapping between the language abstraction of both languages, being able to run the code of each language.

### Background and Literature

[1] Fundamental Proof Methods in Computer Science: A Computer-Based Approach. MIT Press, 2017. K. Arkudas and D. Musser
[2] Programming Elixir. Pragmatic Bookshelf, 2018.  D. Thomas.

### Contact

- m.sanabriaa
- n.cardozo
