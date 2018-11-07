---
title: Abstract interpretation of Rust Programs
period: 2019
level: master
area: pil
abstract: Generate a graph comparison algorithm to unify Rust code
people: Nicolas Cardozo, Christian Poveda
file: cesk_mir
---

### Context
The Rust programming language intends to provide a memory safe alternative to C and C++ for systems programming. This language breaks completely the traditional trade-off between performance and safety by having a compiler able to reason about memory usage and avoiding the need for garbage collection [1].

When compiling code in Rust, the code is transformed into several internal representations: [2]
- First, the code is transformed to a high-level intermediate representation (HIR) where some parsing and desugaring is done
- Second, the code is transformed to a mid-level intermediate represenation (MIR) which is a simple language with a continuation-passing syntax style.
- Third, the code ins transformed into the LLVM intermediate representation and then is compiled by LLVM.

To improve the ergonomics of the language, certain modifications must be done to the manipulations of the internal representations of the language, in particular is necessary to unify expressions of the MIR. However, MIR is a rich, imperative language [3] and as such, traditional methods for unification used in functional and declarative languages will not work here, proper unification requires more advanced techniques.

### Project proposal
This thesis will be based around two central candidates to solve the unification problem: Writing a MIR interpreter based on a CESK machine ,[4] or implement a value state dependency graph representation [5] for the MIR. After deciding which representation is better suited for the problem, traditional unification over such representation should be easily implementable. 

### Implementation plan
The implemetation of the representation and unification algorithms should go as follows:
- Study both the advantages and disadvantages in terms of performance of using CESK machines and VSDG representations.
- Select the better candidate an implement an algorithm to transform the MIR into such representation.
- Implement a traditional unification algorithm.

### Background and Literature
- [1] The Rust Programming Language. Steve Klabnik and Carol Nichols, 2018.
- [2] https://blog.rust-lang.org/2016/04/19/MIR.html
- [3] https://github.com/rust-lang/rfcs/blob/master/text/1211-mir.md
- [4] [Cesk] (http://matt.might.net/articles/cesk-machines/)
- [5] https://www.cl.cam.ac.uk/techreports/UCAM-CL-TR-705.pdf
