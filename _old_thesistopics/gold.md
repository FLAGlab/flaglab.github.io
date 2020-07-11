---
title: Make Gold great again!
period: 2020
level: undergrad
area: pil
abstract: Gold has been used in the LyM course for the past years. Gold can be extended with different automatons. The idea is to determine what extensions are worthy and to implement and deploy the new  version of Gold.
people: Silvia Takahashi, Nicolas Cardozo
file: gold
---

### Context
You probably used Gold [1] to develop automaton-based programs. The version of Gold you used, is already over 6 years old, requiring a well deserved lift-up at different levels. Internally, the language is implemented based on a complex architecture based on model transformations. Externally, the language diverges from the notions of the base-language or a particular programming paradigm. 
The objective of this project is to update and improve Gold so that it can cope with the standards of top Domain-Specific Languages (DSLs) [3].
From the perspective of a Gold user, this is not the most exiting. However, from the perspective of a programming language designer, there are several challenges to tackle. 
1. Gold's syntax requires an update, it should be more natural with respect to its underlying host language.
2. The semantics need to be extended (e.g., to deal with Turing machines, Petri nets, extend the interaction with currently supported automaton) 
3. The interaction with users need improvement (making the API more clear and straight forward).

### Project proposal
This thesis requires technical work involving (the development of) knowledge about Labelled Transition Systems (a.k.a state machines), Object-(functional) programming, DSL and programming language (PL) design and implementation. 
We will revive Gold implementing as an internal DSL of the the Scala programming language [2].
On top of the technical work, the thesis development will (ideally) be accompanied with the specification of the language semantics to prove different properties about the language and its computability.

### Implementation plan
This project will be based on the implementations of Gold as an internal DSL in the Scala programming language. To do this, you will have to follow these stepes.
1. Get familiar with Scala and DSL definitions in Scala
2. Port the basic ideas of the data structures and algorithms currently implemented in GOLD to the new DSL
3. Extend GOLD with new features to ease the development of automata nad Turing machines

### Background and Literature
[1] Gold - [thesis](https://profesores.virtual.uniandes.edu.co/~isis1106/dokuwiki/lib/exe/fetch.php?media=tutoriales:gold3_documento.pdf)

[2] Scala - [https://www.scala-lang.org](https://www.scala-lang.org)

[3] DSL - Domain-Specific Languages: An Annotated Bibliography. A. van Deursen and P. Klint and J. Visser, 2000

### Contact
stakahas

n.cardozo