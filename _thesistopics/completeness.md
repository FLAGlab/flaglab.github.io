---
title: Completeness analysis for JavaScript programs
period: 2021
level: master
area: pil
abstract: Evaluating completeness of JavaScript programs based on a completeness enhancement of the points-to analysis
people: Nicolas Cardozo
file: completeness
---

### Context

Large software projects use different third-party libraries within their development, or call remote components or services defined within the same development group/company. Taking into account the dynamic environment of systems using JavaScript, these third-party modules or services can be loaded dynamically, asynchronously, or lazily as needed. However, managing access to those resources that are not available all the time in the application's runtime can be complex, opening the opportunity for execution failures, caused by the attempt to access an object or service. that is not yet available.

### Project proposal

In order to reduce run-time erros that may present through the execution of a service/function not currently available at run time, the purpose of this project is to implement an integrity analysis [1] for JavaScript. The idea of ​​this type of analysis is based on the construction of the point-to analysis [2], together with techniques of identification of accesses and modifications to the attributes of objects.

Furthermore, we want to apply such techniques for a type of dynamic languages, Context-oriented programming (COP) languages [3], in which particular functions/atributes of an object may appear/disappear unannounced.

### Implementation plan

The base of this project relies on the implementation of completeness analysis [1] for (a subset of) JavaScript using [WALA](http://wala.sourceforge.net). Having this analysis we will move to analyze COP programs for the dynamic completeness analysis of systems with such technology.

### Background and Literature

[1] Completeness Analysis for Incomplete Object-Oriented Programs. Compiler Construction. 2005. Jingling Xue, Phung Hua Nguyen.
[2] Liang D, Harrold MJ. Efficient points-to analysis for whole-program analysis. In Software Engineering—ESEC/FSE’99. 1999 Sep 6 (pp. 199-215). Springer, Berlin, Heidelberg.
[3] González S, Mens K, Colacioiu M, Cazzola W. Context traits: dynamic behaviour adaptation through run-time trait recomposition. In Proceedings of the annual international conference on Aspect-oriented software development 2013 Mar 24 (pp. 209-220).

### Contact

- n.cardozo
