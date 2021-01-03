---
title: Swift ANTLR generic parser
period: 2021
level: undergrad
area: pil
abstract: Build a grammar and parser for the Swift programming language.
people: n.cardozo
file: swift-parser
---

### Context

Parsing is the first step in the analysis of programming languages. For example, to analyze the quality of software systems we can use code clone analysis metric, which detects the percentage of copied code in a program.

To perform such analysis we are first require to encode all the grammar rules of the programming language, and then build a parser that, using our defined grammar, can recognize any program written in the language. Parsers return a tree like structure that is then use as input for our desired static analysis tool.

Thankfully, we do not need to generate full parsers for programming languages, as this task is very complex. We can use existing parser generators, as ANTLR, that, given a grammar, can generate and efficient and correct parser for a language.

In this project we want to use such a parser to analyze mobile application, in particular mobile applications targetting the iOS platform. Therefore, we will focus on the development of a grammar for the Swift language.

### Project proposal

The objective of this project is to define the grammar for the lattests specification of the swift language [(5.3)][https://docs.swift.org/swift-book/ReferenceManual/AboutTheLanguageReference.html]. The grammar must comply with the [ANTLT4][https://www.antlr.org] parser generator specification, with the objective to generate a parser for swift.

### Implementation plan

1. Study the ANTLR 4 specification
2. Study the Swift 5 language reference
3. Define the Swift grammar using ANTLR
4. Evaluate the grammar generatign an effective parser for Swift
5. Generate a corpus of mobile applications built using Swift
6. Evaluate the generated parser using different mobile applications developped in Swift

### Background and Literature

1. Swift language documentation: <https://docs.swift.org/swift-book/LanguageGuide/TheBasics.html>
2. ANTLR parser generator documentation <https://pragprog.com/titles/tpantlr2/the-definitive-antlr-4-reference/>

### Contact

n.cardozo
