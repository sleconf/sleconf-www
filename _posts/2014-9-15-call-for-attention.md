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

One more impression, if you look at parser combinators all the "squiglies" for different kinds of prefix and infix and postfix operators are hard to avoid. So here's a slogan: "Parser combinators are to EBNF what Perl is to Haskell" :-) Don't throw tomatoes.

### 12:00

Now Jan Kurs talks about Island Grammars. Fixing the problems of Island Grammars. And there are many problems with island grammars as we all know. Eelco just whispered in my ear that even ANTLR now has support for Island Grammars.

Greediness is the enemy of island parsing. Jan has a sinking ship or island on his slides. To fix these problems follow restrictions ("predicates") are used to prevent water to overrun the text that we are interested in. This is problematic: now we have the worst of regular expressions combined with the worst of context-free grammars. We don't know which language we accept anymore: it's magic.

Jan's solution is a notation which resembles skeleton grammars a bit and its conceptually clear. The implementation is by using automatic follow restrictions on the boundaries of water.

### 15:00

Sorry for the gap. Emergencies happen :-) Markus Voelter presented his work on evaluating the improvements in MPS for usability. This was quite interesting and I was wondering how often we evaluate UX from the programmers' perspective. The methods used by Markus do not translate easily to textual languages and their IDE's (as he explained) , but I believe the gap is not this wide. 

Now we are listening to a previously recorded talk because the authors could not come (beyond their control). Robert Frans is explaining and also online on Skype. The talk is about #UX of humonguous feature models. Scaling modeling is an interesting topic and ways heavily on the discussion between text and graphical representations. 

Yes, indeed: now Frans argues for textual again, which I am biased for, for some reason. This discussion which is often led by Markus Voelter is sometimes fuzzy. Since we are actually talking about the concept of User Experience and we have not been trained in modeling or understanding this concept, the discussion about the usability difference between programming languages and their IDEs as compared to projectional editing and as compared to graphical is not very satisfactory. One thing which is missing in my view is experimental reports on the _baseline experiences_ of programming in textual editors, semantics-directed editors, structural-editors, etc. Then we would have something to compare to. 

Anyway, one thing is sure: MPS is a very cool and smooth tool which makes projectional editing a very attractive alternative. 

### 15:23

We are still listening to Robert Frans and his presentation was well prepared and easy to follow. Luckily! His conclusion is that the graphical notation increases the usability of the feature moduling tool and the quality of output of the tasks of the studied subjects (people). The conclusions are preliminary because the study has some threats to validity in the size of the group of subjects and the size of their tasks in the experimental setup. Future work will show more.

### 16:00

Daco Harkes is not presenting his research on object relational modeling and unifying the OO and the ER models. 


### 16:00

Daco Harkes is not presenting his research on object relational modeling and unifying the OO and the ER models. He proposes a language design which solves many different kinds of issues with the difference between relations and objects. The integrated model offers bi-direction navigation between objects via first class relations and the type system handles multiplicities. Good 

I am wondering what is the solution for the temporal dimension of relations. Maybe that is still coming. No, that was out of scope because its not a requirement of most web-based systems.

### 16:31 

Thomas Kuhne cites Shakespeare "all the world's a stage ...". Nice opening :-)
Then he says: my research had a for me infortunate outcome, the suspense is rising...

The idea is separation of concerns via role based modeling, such that software becomes more maintainable, and adaptable. I.e. you can assign new roles or remove roles from existing objects, even at run-time. This sounds very plausible and its the basic promise of the role based programming we also see in Balzer's work.

The thoughts that pop up: why did we ever bind data to computations in the first place? Here we are trying to separate it all again. OO <sigh>. 

Thomas gave a very nice overview of how features of roles have been evolving in programming and modeling languages in the last 10 years. He harshly judges language designs which do not improve but rather go back on elements of design that he considers good. It's good to have this overview, but the factors of language design are not all present in this discussion. Perhaps the authors made great trade-off discussions in their context and just had to not satisfy Thomas' requirements.

BTW, the unfortunate outcome that Thomas presented was that the literature was fragmented and inconsistent and therefore hard to learn from. Caveat lector :-)

My question to Thomas, since he talked about the problematic state of the literature and the inconsistencies there, did he make sure Friedrich also agrees with his new ontology?

### 17:00

_warning:  biased report :-)_

Mark Hills is talking about his experience building a control flow graph constructor generator (for any given language). He's jumping right into it, since everybody knows what a CFG is here (control flow graph, not context-free grammar).

Its about Rascal code that might be reusable between different languages because its the same all the time for control flow extraction. Reminiscent of Stratego strategies: control flow extraction can be factored as a higher-order strategy with parameters for detecting the relevant AST nodes and then extract the edges of the graph. Here we go the other route, we go generated instead of generic: where a DSL specific for control flow graph extraction is designed and would generate Rascal or any other language to do the task.

The DSL Mark propose is rule-based, identifying language constructors on the left-hand side and generating graph edges on the righ-hand side. Pure and simply elegant stuff.

_Question_: So we can make any kind of graph from a tree somehow with this. Could we let's say, abstract from the concept of control flow and move to generic graphs? Like DeFacto? Answer yes!

_Question_: can this be done generically with a library (Ralf Laemmel) asking. Answer, yes, that is also possible also under the hood of the generated code.

### 18:00 

So the official program has ended (except for the reception with the prizes!) At this point everybody is either quickly catching up with work, or family, or (and this is a great sign) people are huddled together in discussion groups shop talking, exchanging citations and ideas on the future of SLE. Great!

### 19:00

The best reviewer of SLE 2014 was Emilie Balland from INRIA Bordeaux. Unfortunately she was not able to attend but the quality of her reviews was considered to be the best and Benoit will convey the 100 euro prize to her.

The best  paper was won by "A SAT-based Debugging Tool for State Machines and Sequence Diagrams", P. Kaufmann, M. Kronegger, A. Pfandler, M. Seidl, M. Widl. The prize was 500 euro worth and just-in-time Magdalena Widl arrives to accept it.

The best student paper was awarded to "The Moldable Debugger: a Framework for Developing Domain-Specific Debuggers", A. Chis, T. Girba and O. Nierstrasz. The prize was 500 euro again and we wish Andrei a bright future, expecting to see many more exciting results from him in the SLE conference.

### 24:00

We had a very nice dinner and then some drinks in the hotel. I learned about what is happening in Saarbrücken concernig GPU and FPGA generated code from functional programs for example, while exchanging at the same time epistemic puzzles.