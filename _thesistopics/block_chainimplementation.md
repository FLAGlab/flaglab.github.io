---
title: A Better Blockchain for All
period: 2020
level: undergrad
area: algorithms
abstract: blockchain sucks. Imagine how famous you would get if you actually provide a good implementation of the underlying data structures. Claim your fame, complete your thesis
people: Nicolas Cardozo
file: block_chainimplementation
---

### Context
Blockchain [2] is the biggest hypework in computer science at the moment. Yet nobody knows what it is, let alone how to use them, when to use them, or in which situations to use them. That said, blockchain is pretty useless outside of bitcoin 5 years ago; today ..... not so much.

More over, using a computer scientist hat, any third semester student can easily see that a blockchain is not ideal. Who was the genious that thought of having a distributed data structure in which each node has a pointer to all the previous nodes... well done.

How about all those security features blockchain promises? Well they are still relevant, and is not the worst idea in the world, just the worst implementation. So we can do better.

### Project proposal
The purpose and work of this thesis is to implement the GHOST protocol. The Greedy Heaviest Observed Subtree (GHOST) [3] is an innovative datastructure that implements the blockchain protocol, solving some of the difficulties identified in blockchain. In particular GHOST address the following issue:

Blocks take considerable time to propagate through the network. This raises a problem whenever two minners, called A and B are mining for blocks concurrently (as is expected in distributed systems). Fo example, if A mines a block and B happens to mine another block before miner A's block propagates to B, miner B's block will end up wasted and will not contribute to network security. 

GHOST solves this issue of network security loss by including stale blocks in the calculation of which chain is the "longest". This means that not just the parent and further ancestors of a block, but also the stale descendants of the block's ancestor ("uncles") are added to the calculation of which block has the largest total proof of work backing it.
Ethereum implements a simplified version of GHOST which only goes down seven levels. Specifically, it is defined as follows:

*	A block must specify a parent, and it must specify 0 or more uncles.
*	An uncle included in block B must have the following properties:
*	It must be a direct child of the k-th generation ancestor of B, where 2 <= k <= 7.
*	It cannot be an ancestor of B.
*	An uncle must be a valid block header but does not need to be a previously verified or even valid block.
*	An uncle must be different from all uncles included in previous blocks and all other uncles included in the same block (non-double-inclusion).


### Implementation plan
The implementation of the project will be in Go [1]. 
Once the implementation of GHOST is finished, you will have to provide.

### Background and Literature
- [1] https://golang.org
- [2] X. Xu et al., “A Taxonomy of Blockchain-Based Systems for Architecture Design,” in 2017 IEEE International Conference on Software Architecture (ICSA), 2017, pp. 243–252.
- [3] https://eprint.iacr.org/2013/881.pdf


### Contact
- n.cardozo
