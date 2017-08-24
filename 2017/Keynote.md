---
layout: default2017
title: Keynote - Peter D. Mosses
published: true
---

### Keynote: Engineering meta-languages for specifying software languages

The programming and modelling languages currently used in software engineering generally have plenty of tool support. But although their syntax is specified using formal grammars or meta-models, complete formal semantic specifications are seldom provided.

The difficulty of reuse of parts of semantic specifications, and of co-evolution of such specifications with languages, are significant drawbacks for practical use of formal semantics. I have collaborated in the development of several meta-languages for semantic specification, aiming to eliminate such drawbacks: action semantics, and modular variants of structural operational semantics (MSOS, I-MSOS); this led to the PLanCompS project and to CBS, a meta-language for component-based semantics.

The components of language specifications in CBS correspond to so-called fundamental programming constructs (funcons). The main feature of CBS is that each funcon is defined once and for all: the addition of new funcons does not require any changes to previous definitions, and behavioural laws are preserved. In contrast to software packages, the definition of each funcon has to remain fixed after its publication.

As well as explaining how component-based semantics achieves these desirable pragmatic properties, and comparing its features with those of some other meta-languages, I will demonstrate the current tool support for CBS, which is implemented in Spoofax.