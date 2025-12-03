---
title: Clone detection for UI elements
period: 2026
level: undergrad
area: PiL
abstract: Detection of code clones across interface elements for Kotlin and Dart codebases
people: Nicolas Cardozo
file: uiclones
layout: default
---

### Context

One of the commmon problems in mobile developping is the replication of applications in the different existing platforms (famously iOS and Android). Usually development teams are faced with the decision of keeping two code bases (managed by two development teams) or using code generation frameworks, to deliver applications for all mobile platforms.

There are two problems with maintaining different code bases for the different platforms. First, developers need to ensure that the features in each of the platforms are equivalent. Second, the knowledge of bugfixes in one platform, needs to be transfered to the other platforms.

### Project proposal

To solve this problem we propose a code analysis technique called **code cloning** [1]. We will reause clone-detection software across different languages, and extended to work with kotlin and swift code bases. The tool will be able to identify code similarities between iOS and android applications.

Code clones are usually identified across behavioral elements of programs (that is, the main application logic). However, little to no work exist for the user interface. This problem is particularly problematic for mobile development, where applications' UI are built using external languages (e.g., xml). With new developments on code-oriented UI development, we can extract information about  codebases in different programming languages for the UI elements.

### Implementation plan

The implementation plan of this thesis is focused on the extension of the Out Of Step platform [2]

- Clone detection
  - Extend the kotlin and dart grammars in ANTLR4 to take into account UI elements
  - Test the clone detection algorithm between programs in both code bases in the UI layer of mobile apps
  - extend the corpus of iOS and android applications
  - Evaluate the similarity between applications

### Background and Literature

- [1] Clone detection
- [2] Out Of Step:  https://www.sciencedirect.com/science/article/pii/S0167642324000352

### Contact

n.cardozo
