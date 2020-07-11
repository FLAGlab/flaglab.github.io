---
title: Rogue One: A Phishing Story
period: 2020 
level: undergrad
area: ai
abstract: Analyzing privacy policy agreements to detect rogue and legitimate websites 
people: Nicolas Cardozo
file: privacy
---

### Context

There are over 2 billion websites with over 150 thousand more websites being added daily. These websites are of all types and purpuses, and this being the internet, there is no shortage of malicious websites out to get you (and your information). However, many of these sites are not evil hacker sites as you would imagine. "Respectable" sites may use interesting loopholes in their privacy policy agreements to manipulate your data in a way usually undesired by you.

### Project proposal

In this project we will an extra protection layer for your data by identifying those websites that are safe, may use your data to an extend, or are plain-out stealing your information, based on the declaration of their pricvacy policy.
To do this, we will use Natural Language Processing (NLP) [1,2] algorithms to analyze and classify privacy policies of webpages a multitud of webpages. The objective of this classifications is to identify patterns in privacy policies that can point out whether a website is legitimate or rogue. Some of the privacy policy to analize are:

- Length
- Language used (commonality of words)
- Language structure
- Law fullfillment (location-based)
  - Law presentation and use

### Implementation plan

In order to successfully implement this project you are required to

1. Create a corpus of privacy policies of webpages, both legitimate and rogue

2. Gather information about the privacy policies (sectorized by country/region)

3. Implement an NLP algorithm to analyze the structure of privacy policy documents

4. Implement a webbrowser extension to analize webpage's privacy policies and recommend visit protocols to users


### Background and Literature

[1] Natural Language Processing for Online Applications: Text retrieval, extraction and categorization.
[2] Combining NLP Approaches for Rule Extraction from Legal Documents - https://hal.archives-ouvertes.fr/hal-01572443/

### Contact

n.cardozo
