---
layout: post
published: true
title: SLE call for attention
author: Jurgen Vinju
authorlink: "http://homepages.cwi.nl~/jurgenv"
---

Welcome to the 7th International Conference on Software Language Engineering.

---

### 7:30am

This is a semi-live blog from the audience of SLE. We are in parallel sessions with GPCE and it is clear that we've been working together as a team uptil now, but from here on we are in competition for the attention of the audience :-)

What is SLE to us, the community? It is a conference where artificial boundaries between sub-fields in software engineering have been lifted. The language perspective on software engineering is unifying. 

SLE is a community in which we freely switch between _technological spaces_ -even studying them from a distance- not bound by any socio-cultural limitations. This generates the cross-overs and AHA!'s that bring us a deeper understanding of what software is and how we may predict and control its quality.

We study language engineering without exceptions, for example:

   * SLE provides the computer science perspective on _model driven engineering_ 
   * SLE is the generalization of compiler construction conferences to _metaprogramming_ in-the-large.
   * SLE introduces a programming languages perspective on _information engineering_
   
I hope you will enjoy the 7th instance of SLE. Please feel free to provide any constructive feedback that we may use to make it even better.

### SLE 2014 starts at 8:30 in the room called "Hörsalen".

--- 

### 9:00am

Colin Atkinson bridges viewpoint engineering to language engineering in his invited talk. It's about time! It emphasizes that the language view on software engineering also includes the field of software architecture.

### 9:30am

Colin opens the discussion and puts up a few interesting visions to agree or disagree with:

   * language engineering will be viewpoint engineering in the future
   * software engineering will be governed by viewpoint engineering in the future
   * Summarized by "orthographic software modeling (OSM)"; orthogonal, compositional projections on the same software. An integral idea of which is completeness.
   
_Its interesting that Colin does not see code as a projective view. Is a view just  code (like SLE looks at it), or is code just a view?_

### 9:45am

Colin Atkinson's talk is full of nuggets of insight. Have a look at the slides later if you have missed this. Also check the @sleconf twitter stream.

For example, "heritage, containment and classification", which Colin claims to have to be made explicit (perspecuity) for any model element, remind me of principle design elements of not only modeling languages but also programming languages and their IDEs. Where is code derived from (import, inheritence), where does it reside (files, namespaces), what kind of code is it (methods, classes, data, control)?

"Omission perspecuity" (making clear the difference between something that is missing, placeholders, and actually non-existent). Is this where (programming) languages use formal parameters or templates with holes? So that confirms what Colin is saying: language engineering should start supporting viewpoint engineering. Perhaps this interpretation is to low brow: views should have formal parameters? Opinions appreciated.

### 10:00am

Question from the audience: ok there is this platonic integrated core model of the software "the sum", but what about the constraints between the different orthographic projections? 

_Answer (interpreted by y.t.): well, the constraints should be part of the projections somewhere. the sum is complete and redundancy free.

Question: what about lossy abstractions in the views? like metrics for example?

_Answer (interpreted by y.t.)_: well, the trick is that we have to make the sum stored somewhere to be able to solve partiality caused by abstraction.

Question: language technology can have an important role in defining the "sum". Its good to have large part of the sum as "text" and not hidden as a semantic object which is hard to standardize.

_Answer_: yes, for example togetherj did this. But we have to led go that code and textual form is superior. That's a historical accident. "You can model Java code". There is a more fundamental set of concepts than what is in programming languages. 

(Note: I couldn't disagree more. Programming language concepts are not in the surface syntax, they are just as the concepts he is talking about, fundamental to the way we think and explain things to computers and each-other)

### 11:35

I popped in at the end of Tony Sloane's talk on integrating term rewriting and attribute grammars as embedded in Scala, and Tom Ridge went after explaining what a correct parser actually is and how one would mechanically prove this.
This emphasized a mathematical view on what a parser is and what the set of parse trees is that a parser should produce. 

It is indeed interesting when reading about parsing algorithms that the definition of what soundness and completeness for a parser actually is, let alone complexity analysis, is not at all consistent, neither over different (recent) papers, nor over time. I believe Adrian Johnstone and Elizabeth Scott have reminded us of this fact at the SLE conference as well in the past.

Noteworthy is that Tom sticks with a definition of correctness which can only be satisfied by generalized parsing algorithms.

BTW, next to correctness proving, Tom presents how combinator parsing with "side-effects" (counting wiht memoization) can still be polynomial as opposed to exponential by memoizing the "side-effects" themselves. 