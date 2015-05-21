
---
title: Sujets de recherche - Research Topics
subject: Une synthèse des différents thèmes de recherche explorés.
author: Plume Webmaster
timestamp: 2012-02-12 07:23:44 +0200
tags: 
---

### Summary

The research carried out by the members of the Plume team is mostly centered on two strongly intertwined themes: the _foundation of programming languages_ (design, semantics, implementation, etc) and the _theory of computing systems_ (compositional analysis, security, verification).

International conferences announcing novel results in these areas include: LICS, ICALP, POPL, CONCUR, CSL, ETAPS.

#### Theme 1: The foundation of programming languages




##### ciao

The first theme
revolves around logic, and more specifically proof theory, seen as a guideline for the investigation of the foundation of
programming languages and of their semantics. The second theme focuses on computing systems as an object of study
which we analyze by borrowing tools coming from categorical semantics and logic again.



We are interested in _Proof theory_ and in the _formal semantics_ of programming languages. An important part of the research work of members of the Plume team is related to the deep connections between these two fields.

Such connections are established, at the foundational level, by the *Curry-Howard* correspondence_. According to this correspondence, writing a mathematical proof is a particular case of program development, and running the program is the counterpart of the simplification of the proof. Among the offsprings of this area of research are programs for the computer assisted development of proofs, such as [ Coq][8]. Such systems make it possible to verify properties of programs and to extract a program from the proof of its correctness.

Our research efforts are deployed along different aspects of the *Curry-Howard* correspondence:

##### Proof theory

We are developing modern approaches to proof theory, based in particular on linear logic and game semantics. Our main focus is the analysis of the computational structure of formal proofs in classical logics.

##### Realizability

We use realizability to analyse the computational dynamics of mathematical proofs, seen as programs. This is useful in particular to find new directions for the automatic extraction of programs from proofs.

##### Programming languages semantics

We study formal descriptions of various progamming paradigms/phenomenas (concurrency, pattern matching, randomized algorithms, modularity).

##### Logical approaches to implicit complexity

Implicit complexity is the study of programming constructs which guarantee complexity bounds on program execution and allow one to characterize complexity classes. We work on logical approaches to these questions, made possible by the *Curry-Howard* correspondence applied to linear logic.

##### Computer-assisted reasoning about mathematics and programming languages

We are also users of the [ Coq][8] system (developed at INRIA and Univ.
Paris 11), which is a direct offspring of the research at the interface of computer science and logic. We use it as a modeling tool to formalize both mathematical and computer science developments, such as game theory and equilibria, euclidian geometry, and randomized algorithms.

###  Current research areas

####  The Proof Theory of Classical Logic

#####  Linear Logic and Game Semantics

_Game semantics_ allows one to define a precise interpretation of various programming constructs and logical systems. We use game semantics to work in particular on the proof theory of classical logic (and, via the *Curry-Howard* correspondence, its computational content), quantifiers, and applications to type isomorphisms.

_People involved:_O. Laurent

#####  Diagrammatic Approaches

We study the X calculus, that gives a direct operational interpretation of classical sequent calculus.

Moreover, we workl on diagramatic interpretations of the duality between the hypothesis and conclusions of a sequent expressed by linear negation: a given sequent can be interpreted in several ways, depending on the way each formula is viewed as an hypothesis or as a conclusion. We analyze this phenomenon, and in particular we want to understand operationally how these different interpretations are related.

_People involved:_ P. Lescanne with: S. van Bakel (Imperial College, London, UK), D. Zunic

####  Implicit Computational Complexity

The goal of implicit complexity is to define programming languages or calculi with bounded complexity, like for instance the class of programs that terminate in polynomial time (PTIME) in the size of the entry. Put it differently, the aim of implicit complexity is to define criteria allowing one to guarantee statically complexity bounds on programs. Different approaches can be adopted for this: type systems, logics, rewriting, semantics.

In particular, some variants of linear logic, the so-called light linear logics, where computations have a bounded complexity, like for instance PTIME. These make it possible to define type systems where a well-typed programs terminates in polynomial type. In such a situation, type inference can be used to guarantee statically a complexity bound. We work on approaches based on constraints resolution to address the question of type inference.

We also analyse denotational models of light logics (categorical structures, relational model, coherence spaces, game models, ..) in order to derive more abstract presentations of complexity in time.

These works are supported by the french ANR projects NOCoST (2005-2009) and COMPLICE (2009-2012).

_People involved:_ P. Baillot, O. Laurent with: U. Dal Lago (Bologna Univ., Italy), K. Terui (RIMS, Kyoto, Japan)

####  Realizability

Realizability is an extension of a type system, in which the dynamic behaviour of a program, rather than its structure, determines whether it belongs to a given type. Through the *Curry-Howard* correspondence, realizability allows one to relate programs with logical formulas which are not necessarily provable in usual systems. This represents a way to enrich existing proof systems.

#####  Realizability for Classical Logics

We work on _classical realizability_, which has been introduced by J.-L. Krivine to analyse classical logic. In this setting, a program can be put in correspondence with a large class of proofs (from second order arithmetics to Zermelo-Fraenkel set theory). One research direction we are pursuing consists in using classical realizability to extract programs from proofs in classical logic (possibly relying on the axiom of choice) in the Coq proof system.

_People involved:_ A. Miquel

#####  Reducibility and Rewriting

Reducibility is a variant of realizability invented by Girard at the begining of the 70's in order to prove the strong normalization of second order intuitionistic natural deduction (System F). On the other hand, type systems are often used with extensions of the lambda-calculus, which are usually formulated with rewrite rules.

We are interested in the comparison and the understanding of reducibility techniques. More precisely, we focus on computational and observational properties underlying untyped reducibility. Our approach is to compare reducibility families w.r.t. their stability by union and their ability to handle rewriting, and seek at generalizations to other programming paradigms.

_People involved:_ C. Riba

#####  Pattern Matching

We are working on an analysis of the semantics of pattern matching in type theory. Our starting point is A. Arbiser, A. Miquel and A. Rios' lambda- calculus with constructors. This calculus is confluent and satisfies a separation property (like in Boehm's theorem). The goal of this work is to equip this calculus with a suitable type system, which should in particular make pattern matching commute with application and abstraction.

The type systems we work on are analysed using realizability techniques, along the lines of Girard's reducibility candidates.

_People involved:_ A. Miquel, B. Petit with: A. Arbiser, A. Rios (U. Buenos Aires, Argentina)

####  Process Calculi for Mobile and Distributed Computation

We have an expertise in concurrency theory, and, more precisely, on process calculi for the description and the analysis of distributed and mobile systems (most notably R. Milner's pi-calculus).

#####  Behavioural Properties of Processes

We are partiqcularly interested in developing techniques that make it possible to prove properties about the behaviour of processes. Such techniques include operational equivalences, type systems, and modal and spatial logics.

We work on understanding the expressiveness and the fundamental properties of these techniques (axiomatic characterisations, congruence properties of bisimulation, separating power), and on developing techniques for particular properties of processes (notably type systems for termination).

_People involved:_ R. Demangeon, D. Hirschkoff with: D. Sangiorgi (U. Bologna, Italy), N. Kobayashi (Tohoku Univ., Japan), D. Pous (projet Sardes, INRIA Rhône Alpes) As of 05/10 2010, D. Hirschkoff is external collaborator in the INRIA [Focus][9] project.

#####  Dynamic Modularity

We work with the INRIA Sardes project on a calculus designed to model software components. It is a higher-order message-passing calculus with hierarchical, distributed localities, explicit routing of messages, featuring pattern- matching and passivation of components. Our goals including setting up an adequate notion of bisimulation for it, and extending it with a notion of shared component.

This activity is supported by the french ARASSIA initiative (ANR - [Modyfiable][10] project, 2006-2008).

_People involved:_ D. Hirschkoff, A. Pardon with: T. Hirschowitz (U. Savoie, Chambéry), D. Pous, A. Schmitt and J.-B. Stefani, (projet Sardes - INRIA Rhône Alpes), R. Garner (Uppsala, Sweden)

#####  *Curry-Howard* for Concurrency

More recently, _differential nets_ have made it possible to relate proof theory and process calculi. This opens the way for an extension of the *Curry-Howard* correspondence towards concurrent programming. As a first step in this direction, it has been shown that finitary calculi like solos and the pi- calculus can be encoded in differential nets.

Research in this area is in particular funded by the french ANR Project [CHoCo][11] (2008-2010).

_People involved:_ O. Laurent with: T. Ehrhard (PPS, Univ. Paris 7), K. Honda (Queen Mary and Westfield College, London, UK)

####  Formalizations in the Coq Proof Assistant

We use the [ Coq][8] system as a modeling tool to formalize both mathematical and computer science developments.

#####  Constructive Geometry

Hilbert gave the first axiomatisation of planar geometry. From a constructive point of view, the constructions using a compass and a rule described twenty centuries earlier in Euler's Elements seem more appropriate. We try to give a counterpart of this approach in Coq, based on inductive definitions. Points are then constructed as intersections between lines and circles, and can thus be constructed in several different ways. More recently, we started working with L. Vuillon (Université de Savoie) on dicrete planar geometry. Every point is defined using constructeurs, so that lines appear as Bresenham lines.

_People involved:_ J. Duprat with: L. Vuillon (Université de Savoie)

#####  Verification of Randomised Algorithms

Randomised algorithms are widely used either for finding efficiently approximated solutions to complex problems, for instance primality testing, or for obtaining good average behaviour, for instance in distributed computing. They are also often key parts of security enforcement protocols related to cryptographic algorithms. Proving properties of such algorithms requires subtle reasoning both on algorithmic and probabilistic aspects of the programs. Providing tools for the mechanisation of reasoning is consequently an important issue.

As we favour higher-order logic for expressing properties, our approach aims at providing the Coq proof assistant with adequate tools and libraries toward our purpose. From the user point of view, we take the recently introduced probabilistic functional lambdaO-calculus as programming language, and offer program annotations along the same lines as Hoare's Axiomatic Semantics. Coq formulas, a.k.a. verification conditions are generated which take advantage of
Paulin's axiomatisation of the unit interval, which should avoid by design the need for developing a full but hopefully useless library for
Lebesgue Measure Theory.

This activity is supported by [ Scalp][12] ANR project (2008-2012).

_People involved:_ P. Audebaud with: C. Paulin (LRI, Orsay), Everest team (INRIA, Sophia-Antipolis)

#####  Game Theory and Equilibria

Game theory has been introduced by Morgenstern and von Neumann, and then further studied by Nash. It can be seen as the theory of equilibria and rationality. Our goal is to revisit this sixty years old theory taking advantage from recent progress in logic, and with biological models as main application domain.

_People involved:_ P. Lescanne with: F. Delaplace (IBISC, Génopole, U. Evry) and R. Vestergaard (JAIST,
Japan)


[3]: http://www.ens-lyon.fr/
[4]: http://www.inria.fr/
[5]: http://www.univ-lyon1.fr/
[6]: http://www.ens-lyon.fr/LIP/
[8]: http://coq.inria.fr/
[9]: http://focus.cs.unibo.it/
[10]: http://sardes.inrialpes.fr/collaborations/collaborations/modyfiable.html
[11]: http://choco.pps.jussieu.fr/
[12]: http://scalp.gforge.inria.fr/
