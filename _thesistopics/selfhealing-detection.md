---
title: Self-healing Detection mechanisms
period: 2024 
level: undergrad
area: pil
abstract: Detect points of failure for running programs and generate the infrastructure to fix them automatically
people: Nicolas Cardozo
file: selfhealing-detection
layout: default
---

### Context

The estimated cost of maintenance due to software disruptions is over 59 billion per year, which constitutes 60% of the total cost of software projects. Use of validation and verification techniques can reduce maintenance costs down to 23%. Such costs can be further reduced thorugh the automation of software repair tasks. Therefore, with this project we want to further reduce maintenance costs by going beyond existing techniques which target anticipated disruptions, and investigate how to autonomously heal unanticipated disruptions in software systems.

The area of self-healing systems [1] defines software systems that have the capability to discover, diagnose, and recover from disruptive behavior. In such systems it is possible to identify a given error, and automatically repair it, through a predefined healing path for the given error-state. This mechanism works well for known or anticipated errors, that have a clear path to recovery. Managing unexpected disruptions is more challenging, as the disrruption states are unknown beforehand. As a consequence we must explore ways to manage unexpected disruptions taking place at unanticipated states.

We will focus on complex systems with unknown program states (\eg debuggers, multi-tenant systems) and present new healing techniques to render the systems smart, context-aware, and dynamically adaptive.
The systems will become context-aware and dynamic by means of Context-oriented Programming (COP) abstractions to manage behavior adaptations dynamically, in response to information gathered from the execution environment (both internal and external system states) [2,4].

 Los sistemas se volverán inteligentes y autónomos al expandir las técnicas de aprendizaje de opciones para extraer información de contexto y generar adaptaciones dinámicas de comportamiento a situaciones desconocidas [3]. A través de la combinación única de COP y RL, este enfoque novedoso se utilizará para permitir la automatización de las acciones de recuperación del comportamiento disruptivo al comprender las adaptaciones como secuencias de acciones de recuperación que se aprenderán a partir de las observaciones del comportamiento correcto en tiempo de ejecución (por ejemplo, acciones ejecutadas por el usuario). y los contextos como la causa raíz (estado) de las interrupciones. Este esfuerzo conducirá a sistemas de software de autorreparación inteligentes y totalmente dinámicos. La importancia de este trabajo se basa en aumentar la tolerancia / resistencia de los sistemas de software complejos a las interrupciones imprevistas del tiempo de ejecución. En particular en este proyecto nos enfocaremos en el tema de la detección de fallos

### Project proposal

The job of this thesis is to make self-healing systems smarter and autonomous by expanding option learning techniques to extract context information and generate dynamic behavior adaptations to unknown situations [3].
Through the unique combination of COP and RL this novel approach will be used to enable the automation of recovery actions to disruptive behavior by understanding adaptations as sequences of recovery actions to be learned from correct behavior observations at run time (e.g., user executed actions), and contexts as the root cause (state) of disruptions. This effort will lead to fully dynamic and smart self-healing software systems. The importance of this work is anchored in increasing the tolerance/resiliency of complex software systems to unanticipated run-time disruptions.

### Implementation plan

In particularm the work of this theis will focus on the first step in this process. Detecting disruptive behavior to unknown situations. Common techniques to detect disruptions in software systems include the identification of node failures or log monitoring. The student will work on extending detection techniques to go beyond the identification of particular nodes or monitoring execution logs, to extract specific program states and lift them as execution contexts to introduce specialized behavior dynamically [3]. The challenge to address in this phase lies in how to identify disruption states, when multiple recovery action sequences can be applied.

### Background and Literature

[1]. A survey on self-healing systems: approaches and systems. Computing 91.1 (2011). H. Psaier and S. Dustdar
[2] Semantics for Consistent Activation in Context-Oriented Systems. International Journal of Information and Software Technology, 2015.  Nicolás Cardozo, S. Gonzalez, R. Van Der Straeten, K. Mens, J. Vallejos, T. D’Hondt
[3] Nicolás Cardozo and I. Dusparic. Auto-COP: Adaptation Generation in Context-Oriented Programming using Reinforce- ment Learning Options. arXiv.2103.06757. Tech. rep. 2021.
[4] Modeling and analyzing self-adaptive systems with context Petri nets.  International Symposium on Theoretical Aspects of Software Engineering. 2013. Nicolás Cardozo, S. González, K. Mens, R. Van Der Straeten, T. DHondt

### Contact

- m.sanabriaa
- n.cardozo
