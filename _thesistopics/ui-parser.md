---
title: Parser builder for mobile UI programs
period: 2021
level: undergrad
area: pil
abstract: Extend the grammar of a mobile language to include features strictly related to the UI. 
people: Nicolas Cardozo
file: ui-parser
---

### Context

A lot of the software development now a days is moving towards mobile. However, the tools and quality assurances practices have not move at par with the icnreasing codebases. As a result, the type of analyses that exist targeted to mobile platforms is limited. Evenmore, the different platforms and programming languages for mobile development make it more complicated to build  analysis tools for mobile programs.

To counter this, we can use the grammar rules of the programming language, build a parser that can recognize any program written in the language, and using the parser build an appropriate structure (e.g., AST) to analyze the program.

Such process is already exists for the base language grammars. However, these leave out of scope the graphical aspects of the system, which in mobile systems play a very important role.

In this project we want to use extend the grammar of the mobile programming languages to include aspects of UIs, in order to extend the possibility of analyzing quality attributes of the system that include the UI. This objective is now possible with the effort from mobile platforms to enable the definition of UIs programamtically (e.g., SwiftUI, google UI toolkit)

such a parser to analyze mobile application, in particular mobile applications targetting the iOS platform. Therefore, we will focus on the development of a grammar for the Swift language.

### Project proposal

The objective of this project is to define the grammar and parser that extends the lattests specification of the mobile programming languages (i.e., Kotlin, Swift, Dart). Thankfully, we do not need to generate full parsers for programming languages, as this task is very complex. We can use existing parser generators, as ANTLR, that, given a grammar, can generate and efficient and correct parser for a language. Therefore, the grammar definition must comply with the [ANTLT4][https://www.antlr.org] parser generator specification.

### Implementation plan

1. Study the ANTLR 4 specification [1]
2. Study the mobile language grammar specification (Kotlin, Swift, or Dart)
3. Study the programmatic aspects UI development or the language (google toolkit, SwiftUI, Dart)
4. Extend the langauge grammar using ANTLR to include UI features
5. Evaluate the grammar extension generatign an effective parser for Swift
6. Generate a corpus of example UI features to evaluate
7. Evaluate the generated parser using the corpus of mobile features

This topic is offered to 3 students, each working on one of the mobile languages

### Background and Literature

1. ANTLR parser generator documentation <https://pragprog.com/titles/tpantlr2/the-definitive-antlr-4-reference/>

### Contact

n.cardozo
