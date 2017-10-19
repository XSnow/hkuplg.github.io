---
layout:  post
title:   "Unifying Typing and Subtyping"
authors: "Linus"
date:    2017-10-20 10:00:00 +0800
venue:   "CB 313"
categories: Linus 2017
---
## Abstract

In recent years dependent types have become a hot topic in programming language
research. A key reason why dependent types are interesting is that they allow
unifying types and terms, which enables both additional expressiveness and
economy of concepts. Unfortunately there has been much less work on dependently
typed calculi for object-oriented programming. This is partly because it is
widely acknowledged that the combination between dependent types and subtyping
is particularly challenging.

This talk presents λI≤, which is a dependently typed generalization of System
F≤. The resulting calculus follows the style of Pure Type Systems, and contains
a single unified syntactic sort that accounts for expressions, types and kinds.
To address the challenges posed by the combination of dependent types and
subtyping, λI≤ employs a novel technique that unifies typing and subtyping. In
λI≤ there is only a judgement that is akin to a typed version of subtyping. Both
the typing relation, as well as type well-formedness are just special cases of
the subtyping relation. The resulting calculus has a rich metatheory and enjoys
of several standard and desirable properties, such as subject reduction,
transitivity of subtyping, narrowing as well as standard substitution lemmas.
All the metatheory of λI≤ is mechanically proved in the Coq theorem prover.
Furthermore, (and as far as we are aware) λI≤ is the first dependently typed
calculus that completely subsumes System F≤, while preserving various desirable
properties.
