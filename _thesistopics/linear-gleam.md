---
title: Linear types for Quantum computing in Gleam
period: 2025
level: undergrad
area: PiL
abstract: Develop a linear type system in gleam to be used in the development of Quantum computing programs
people: Nicolas Cardozo, Daniel Barrero
file: linear-gleam
layout: default
---

### Context

Software verification at the type system level is used to check that programs are sound ahead of time. the idea of type systems is that if programs type-check, they will execute properly (or their strange behavior will be outside of the type system). Linear types [4], are a particular type system in which variables must be used exactly once in a program.

This idea is of particular interest in the case of Quantum programming, as one of its prperties is that as soon as a q-bit is observed, it cannot longer be used.

### Project proposal

the objective of this project is to incorporate the ideas of linear types to a new functional programming language, Gleam [3], a BEAM-Elixir [1] compatible language.

With a linear type system, it will be possible to implement Quantum programs using Gleam (based on existing Elixir libraries), that can be verified for properties as the use of q-bits, or to verify quantum cryptography protocols.

### Implementation plan

The implementation plan for this project is:

1. Understand the theory of linear types
2. Get familiar with Gleam
3. Extend Gleam to incorportate linear types
4. Build a quantum application using the linear types extension of Gleam

### Background and Literature

[1] Programming Elixir. Pragmatic Bookshelf, 2018.  D. Thomas.
[2] [Quantex](https://github.com/piacerex/quantex)
[3] [Gleam](https://gleam.run)
[4] [Linear Types](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=24c850390fba27fc6f3241cb34ce7bc6f3765627)

### Contact

n.cardozo
dr.barrero2562
