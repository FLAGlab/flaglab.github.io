---
title: Cross-platform clone detection
period: 2023
level: master, undergrad
area: pil
abstract: Detection of repeated/plagearized code between iOS and android applications
people: Nicolas Cardozo
file: clone_detection
---

### Context

One of the commmon problems in mobile developping is the replication of applications in the different existing platforms (famously iOS and Android). Usually development teams are faced with the decision of keeping two code bases (managed by two development teams) or using code generation frameworks, to deliver applications for all mobile platforms.

There are two problems with maintaining different code bases for the different platforms. First, developers need to ensure that the features in each of the platforms are equivalent. Second, the knowledge of bugfixes in one platform, needs to be transfered to the other platforms. 

### Project proposal
To solve this problem we propose a code analysis technique called **code cloning** [1]. We will reause clone-detection software across different languages, and extended to work with kotlin and swift code bases. The tool will be able to identify code similarities between iOS and android applications.

Additionally, we will build a recomendation tool to recommend cross-platform changes. That is, given a change in one of the code bases (say android), the tool will recommend the change and location for the change in the other code base (iOS) 

### Implementation plan

The implementation plan of this thesis is divided in two phases.

- Clone detection
  - Extend LICCA [2] with the kotlin and swift grammars
  - Test the clone detection algorithm between programs in both code bases
  - Extend the tool to evaluate similarity of complete projects
- Mobile clode detection
  - Create a corpus of iOS and android applications 
  - Evaluate the similarity between applications
- Build a recommender system for cross-platform bug-fixing
  - Suggest changes from a code base to the other
  - Pinpoint location of changes based on the similarity detection
  - Suggest a code transformation based on the similarity of the langages

### Background and Literature

- [1] Clone detection
- [2] LICCA [https://www.researchgate.net/publication/323535753_LICCA_A_tool_for_cross-language_clone_detection](https://www.researchgate.net/publication/323535753_LICCA_A_tool_for_cross-language_clone_detection). [code](https://github.com/gocko/licca)
- [3] OOS

### Contact

n.cardozo