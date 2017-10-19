---
layout:  post
title:   "Type-Safe Modular Parsing"
authors: "Haoyuan"
date:    2017-10-20 10:00:00 +0800
venue:   "CB 313"
categories: Haoyuan 2017
---
## Abstract

Over the years a lot of effort has been put on solving extensibility problems,
while retaining important software engineering properties such as modular
type-safety and separate compilation. Most previous work focused on operations
that traverse and process extensible Abstract Syntax Tree (AST) structures.
However, there is almost no work on operations that build such extensible ASTs,
including parsing.

This paper investigates solutions for the problem of modular parsing. We focus
on semantic modularity and not just syntactic modularity. That is, the solutions
should not only allow complete parsers to be built out of modular parsing
components, but also enable the parsing components to be modularly type-checked
and separately compiled. We present a technique based on parser combinators that
enables modular parsing. We show that Packrat parsing techniques, provide
solutions for such modularity problems, and enable reasonable performance in a
modular setting. Extensibility is achieved using multiple inheritance and Object
Algebras. To evaluate the approach we conduct a case study based on the "Types
and Programming Languages" interpreters. The case study shows the effectiveness
at reusing parsing code from existing interpreters, and the total parsing code
is 69% shorter than an existing code base using a non-modular parsing approach.
