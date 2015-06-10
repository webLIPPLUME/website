
---
title: Sujets de recherche - Research Topics
subject: Une synthèse des différents thèmes de recherche explorés.
author: Plume Webmaster
timestamp: 2012-02-12 07:23:44 +0200
tags: 
---

The research carried out by the members of the Plume team is mostly centered on two strongly intertwined themes: the _foundations of programming languages_ (design, semantics, implementation, etc) and the _theory of computing systems_ (compositional analysis, security, verification).


## Theme 1: The Foundations of Programming Languages

- Logical Foundations of Programming Languages

How can _logic_ help in designing languages for writing safe programs?  We investigate  _proof theory_ as a foundation for programming languages and their _semantics_. In this area the _proofs-as-programs correspondence_ has triggered the design of _types systems_, for statically ensuring properties, and of proof assistants, for verifying correctness. _Linear logic_ and _game semantics_ are fundamental tools for these works, and are themselves objects of research. Some examples of challenges are: the definition of game semantics for concurrent languages conveniently crafted to overcome combinatorial explosion problems, and the design of type systems that statically ensure complexity bounds on programs.




## Theme 2: Theory of Computing Systems

How can one specify and formally verify complex computing systems?  We analyse computing systems by using tools from _logic_ and _category theory_. In particular we work on concurrent systems, for which we try to develop _coinductive_ verification methods based on _operational semantics_, as well as the mechanisation of reasoning with these techniques. Concurrency and category theory have also been an inspiration for _rule-based modeling_, a programming paradigm for the representation and analysis of complex systems, in particular in biology.Moreover we also work on theoretical tools for verification: logics, games, algebraic systems. _Monadic second-order logic_ (MSO) is studied from various viewpoints: using model-theoretic as well as proof-theoretic methods and exploring topological and probabilistic aspects. _Game semantics_ is used to develop compositional approaches to model-checking. Algebraic systems for verification such as _Kleene algebras with tests_ (KAT) and their extensions are explored for axiomatisations, decidability issues, and mechanization through the Coq proof-assistant.

**Monadic Second Order Logic.**
Büchi's and Rabin's theorem (1962,1969) constitute fundamental theoretical results and are at the basis of numerous formal verification tools for concurrent systems. Our recent research results on MSO include: full axiomatizations (Riba, Das), new model theoretic proof of classical results (Riba), Lebesgue measurability and closure-properties of regular sets of trees (Mio), algorithms for computing the probability of regular sets of trees (Mio).


