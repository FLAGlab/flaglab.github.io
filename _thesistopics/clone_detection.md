---
title: Cross-language program analysis
period: 2024
level: master
area: pil
abstract: Analyzing structural and quality properties of software systems across programming languages.
people: Nicolas Cardozo
file: clone_detection
layout: default
---

### Context

Software systems are becoming more heterogeneous with respect to their code base. Aditionally, the translation of systems into different codebases is not uncomon. To coope with the incresing complexity, understanding, and translation of multi-language software systems, it is required to generate the tools to manage and analyze such systems.

One possible approach to develop multi-language analysis tools is through the abstraction of the languages into an representation where the syntactic details are hidden away, and keep the structural and software quality attributes of the system.

### Project proposal

In this project, we want to propose a multi-language program analysis tool based on Voronoi diagrams [1]. The objetive of the tool is to analyze programs developed in different programming languages to assess their similarities and differences. Additionally, the tool will evaluate the system's evolution with two purposes, tracking feature divergence, and identidying the effect of refactorings on software systems as linear transformations tranferable across languages.

### Implementation plan

The implementation plan of this thesis is as follows.

- Program abstraction
  - Abstract the representation of programs as Voronoi diagrams using different software quality properties
- Program comparison
  - Design a comparison analysis for program representations
  - Design a comparison analysis across program versions
  - Design an algorithm to detect and track feature divergence
  - Extract the refactorings between program versions with their effect
  - Apply refactoring functions to evolve programs

### Background and Literature

- [1] Voronoi Diagrams [paper](https://dl.acm.org/doi/pdf/10.1145/116873.116880)

### Contact

n.cardozo
