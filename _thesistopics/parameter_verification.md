---
title: Verification of Parameter Passing Semantics in Actor Systems
period: 2026
level: undergrad
area: PiL
abstract: Formal verification of function distribution using pass-by-move semantics in actor systems
people: Nicolas Cardozo, Mateo Sanabria
file: parameter_verification
layout: default
---

### Context

Programming is hard.

There are two paths to help in descovering if programs actually behave as intended. First, there is validation, to state a program works under certain tested scenarios. Validation is generally the result of program testing or proof of concept applications. While validation works well, it does not provide any assurances about the program's behavior. To deal with these situations, there is verification. Verification comos from a formal mathematical proof demonstraiting without a doubt that a program satisfies a given property.

Doing formal proofs for software behavior is contraintuitive. However, we can develop proofs as if we are writing programs through verification languages like Athena [1].

### Project proposal

In this project we are interested in a specific property of concurrent and distributed systems, function mobility. In distributed systems, the pass-by-move parameter passing semantics is defined to enable the move of parameters across nodes. This means that when a function is called with a given parameter, the parameter ceases to exist in the caller's scope, and it is moved into the callee's scope.

We have explored the implementation of pass-by-move semantics as part of the implementation of cloud and distributed applications [3], based on the actor concurrency model in the Elixir language [2].

With this project we want to create an Athena specification of the pass-by-move implementation to verify that, following the specification, functions move successfully, preserving their scope and sound behavior.

### Implementation plan

The implementation of the thesis will be developped in the Athena programming language, to verify explicitly the characteristics of Elixir actors. The implementation will require to:

1. Study formal proofs and the Athena language
2. Get familiarized with Elixir
3. Provide an specification for Elixir actors
4. Specify the pass-by-move semantics
5. Verify the move behavior in Athena

### Background and Literature

[1] Fundamental Proof Methods in Computer Science: A Computer-Based Approach. MIT Press, 2017. K. Arkudas and D. Musser
[2] Programming Elixir. Pragmatic Bookshelf, 2018.  D. Thomas.
[3] [Pass-by-move elixir](https://github.com/FLAGlab/by-move)

### Contact

n.cardozo
m.sanabriaa
