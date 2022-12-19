---
title: Petro nets
period: 2023
level: undergrad
area: pil
abstract: We are going to implement new an interesting was of interaction for Petri nets
people: Nicolas Cardozo
file: petro
---

### Context

Petri nets [1] are well known structures to model the behavior of many different systems, in particular concurrent systems. The basic Petri net model is already expressive enough to be useful for the representation of a hand-full of computational and real life model. Nonetheless, there exist Petri net extensions that alter the common behavior of the base model for a specific purpose, for example to model time with a Petri net.

### Project proposal

In this project we want to extend the Petri nets model with democatrization. That is, we want to modify the behavior of the Petri net model to allow the net to re-distribute its tokens evenly at a given moment in time. The purpose of this new model, called Petro nets, is to model balancing/scheduling/stealing algorithms for multi-processor design.

### Implementation plan

The implementation of the project will consist of the implementation of a full web interface for a Petri net simulator, extended with the Simulation of the newly developed Petro nets. For the implementation, the student must use Rust [2], to develop the web simulator using WebAssembly [3].

The implementation plan consists on:

- Building the basic Petri net behavior
- Extendidn the behavior for Petro nets
- Implementing the web simulator
- Testing the simulator to model balancing algorithms

### Background and Literature

- [1] Petri nets <https://dl.acm.org/doi/pdf/10.1145/356698.356702>
- [2] Rust: <https://www.rust-lang.org>
- [3] WebAssembly: <http://webassembly.org>

### Contact

n.cardozo
