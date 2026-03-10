---
title: A complete C grammar
period: 2025
level: undergrad
area: pil
abstract: Build a grammar and parser for the C programming language.
people: Nicolas Cardozo
file: c-parser
---

### Context

Parsing is the first step in the analysis of programming languages. For example, to analyze the quality of software systems or to perform language transformations.

To perform such analysis we are first require to encode all the grammar rules of the programming language, and then build a parser that, using our defined grammar, can recognize any program written in the language. Parsers return a tree like structure, we will be a specifc kind of tree called eCST [1] that is then use as input for our desired translation tool.

Thankfully, we do not need to generate full parsers for programming languages, as this task is very complex. We can use existing parser generators, as ANTLR, that, given a grammar, can generate and efficient and correct parser for a language.

In this project we want to use such a parser to translate dated C applications into a 21st century language like Rust. The first step in the translation, your project, will be to create an intermediate representation that abstract specific syntactic abstractions for an effective translation.

### Project proposal

The objective of this project is to take the existing grammar definition for C and compliment it with missing features in the language (deprecated or new features). The grammar must comply with the [ANTLT4][https://www.antlr.org] specification. Then, given the grammar, with the objective to generate a parser for swift.

### Implementation plan

1. Study the ANTLR 4 specification
2. Review features missed by the existing C ANTLR4 grammar
3. Extend the C grammar with missing features
4. Generate correct eCST from concrete programas
5. Evaluate the generated parser using different C applications with example programs from the past versions (within the last 30 years)

### Background and Literature

1. Rakić, N., Rakić, G., Sukur, N., & Budimac, Z. (2017, May). eCST to source code generation-An idea and perspectives. In 2017 40th International Convention on Information and Communication Technology, Electronics and Microelectronics (MIPRO) (pp. 570-575). IEEE.
2. ANTLR parser generator documentation <https://pragprog.com/titles/tpantlr2/the-definitive-antlr-4-reference/>

### Contact

n.cardozo
