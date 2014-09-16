---
layout: post
published: true
title: SLE call for attention
author: Jurgen Vinju
authorlink: "http://homepages.cwi.nl~/jurgenv"
---

Welcome to the 7th International Conference on Software Language Engineering.

* all tweets about SLE are here: https://twitter.com/search?q=%40sleconf&src=typd, since they are all mentioning `@sleconf`
* we did not use the #sle2014 hash tag because some marathon people stole it on the first day :-)
* please find pictures of the two SLE days [here](https://www.dropbox.com/sh/denmlgj3b2ksr3f/AABXFADQgiG25_5c62uNfV23a?dl=0)
* the SLE report, day 2, continues <a href="#daytwo">here</a>.

---

## Day one

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

The best  paper was won by "A SAT-based Debugging Tool for State Machines and Sequence Diagrams", P. Kaufmann, M. Kronegger, A. Pfandler, M. Seidl, M. Widl. The prize was 500 euro worth and just-in-time Magdalena Widl arrived to accept it.

The best student paper was awarded to "The Moldable Debugger: a Framework for Developing Domain-Specific Debuggers", Andrei Chis, Tudor Girba and Oscar Nierstrasz. The prize was 500 euro again and we wish Andrei a bright future, expecting to see many more exciting results from him in the SLE conference.

### 24:00

We had a very nice dinner and then some drinks in the hotel. I learned about what is happening in Saarbrücken concerning GPU and FPGA generated code from functional programs for example and we exchanged epistemic puzzles.

## <div id="daytwo">Day Two</div>

Good morning!

### 09:00

Nikolai Tillmann from Microsoft research is the second shared keynote speaker. He will talk about touch develop. Great! He starts with the Commodore 64 Basic  prompt saying "program me!". :-)

Nikolai now says: "Programming languages follow input paradigms", now that drives the discussion about projectional editing home. See yesterday's discussion with Markus Voelter.

The great thing about this keynote is that Nikolai is giving a live demo. TouchDevelop is a projectional editor for HTML5 scripting, but only with program text not images. It is driven by the touch input paradigm and by learning algorithms for online API suggestions. Looks like fun!

"The app store model is not the best way to share creativity fast", with TouchDevelop you can share your code fast. The code is in the public domain the moment you publish your app.

Since TouchDevelop collects statistics about language usage and also about usage of your app it really and finally brings Knuth's vision of learning from language use to the mainstream. Knuth proposed this long ago in this 1971 paper:
```
D. E. Knuth. An Empirical Study of FORTRAN Programs. Software: Practice and Experience, 1(2):105–133, 1971.
```

Another part of the story of programming language experience is library design. Here TouchDevelop goes the WebDSL route, where the most important libraries for application development are integrated linguistically: data binding, UI elements, events.

On a personal note; I have developed a lot of applications with Ms. Access. It had a kind of immediacy and integrated feeling "everything at your fingertips". Ever since I learned about web programming I wanted to go back to this experience. I thing TouchDevelop does this and goes quite a bit further. 

Otherwise now we are going into sales pitch mode. The thing is nice and has lots of features. What do we learn from all this? Well, the internet has definitely come to programming and its not going away anymore. The internet connectivity is now _necessary_ to able to effectively work with your IDE. 

Cool: now we can chat with him [online right now](http://tdev.ly/sjdi) using his own app he just online developed during his keynote. So we're all sold on this :-)

We now move to the education _viewpoint_. The tutoring environment is totally interactive and scripts the learning experience. It makes you go through the moves of creating an app and you get cudo's. Of course we want this for all of our tools and I wonder if we can have generic or generated tutoring functionality.

_Now the pressing question from the SLE perspective_: what kind of language engineering is fundamental to this entire TouchDevelop experience, including "tutoral engine", etc. We will ask him during the break.

One answer: we get data immediately from our users and use this to improve our language design. One lesson: speech is also a good way to program! 

Open challenges for Touch Develop:
   * tree diff
   * real-time collaborative editing
   * running server side code
   
### 10:30

We continue with SLE and immediately dive into technological spaces: interoperability between modeling platforms with the paper "UML as an Assembly Language for Model Transformation". 

"A modeling virtual machine (MVM) abstracts from programming language and modeling framework"

fUML serves as the MVM. The case study is to port ATL to fUML and see if this satisfies the requirements of having a VM and inter-operability etc. Interesting!

I am waiting to see if we take a modeling language which is not OO but rather algebraic/functional. And while listening I am wondering how we test the compilers or even verify them. Let's see.

Wait: the conclusion of this research is interesting: the Java VM is a better option now for modeling interoperability. 

### 11:01

Now "Dynamic Scope Discovery for Model Transformation". It's about a performance model for graph-based model transformation. It makes a heat map of the nodes which are being matched. This can be used to strategically search for matches with a higher chance of success using machine learning.

### 11:24

Next up: "ProMoBox: framework for generating domain-soecific property languages"

### 12:00 

Panel Discussion!

* Anya Helee Bagge starts of and explains how her experience shows that students learn more about semantics of programming from the SLE course than SLE concepts per sé.
* Jaakko Järvi says that SLE is also about the fact that programs are malleable things and there exists a toolbox for this. The current curricula don't have this aspect and students are missing out because of that. Where do we put this?
* Ulrik Schultz teaches roboticists and Java programmers (bachelors). He learns them internal and external DSLs and the students are motivated by the fact that they are learning how languages work. The few computer science students he has get a different perspective on compilers as well. Ulrik in effect agrees with Anya in this. Eclipse is too complex. You can learn DSLs without knowing about programming languages.
* Anthony Sloane: has been teaching a cross-over between compiler and SLE. From hard core back-ends to front-end and API and modeling. The goal is to focus the students minds on the commonality between languages. Scala is used for the implementation (Kiama for attribute grammars and term rewriting). They see a lot of stuff without seeing lots of code. They build type systems and translators.
* Massimo Tisi teached Model Driven Engineering and Domain Specific Modeling Languages. They use language workbenches and then a project where the students have to design a new language. The problem is that although the students like the tools, the language _design_ is the problem. They don't know how to shape the abstractions. This is harder than API design because in other courses the students can design an E/R model or an OO model, but the language abstraction seems a bridge too far.
* Eric Van Wyk: traditional compiler courses are valuable too. Understanding how a compiler works makes people better programmers. We have a new second year course on advanced programming principles: Programs as data, ADTs, representing complex hierarchically structured data (ASTs). And in another course we build little compilers. Little things like ASTs are enlightening for the students.

---

* Discussion from the audience: better languages, safer languages is what we want the students to learn about and think about. Ralf asks what other things should SLE education would be about? Answers:
   * data is software too. Anya we include data formats, ontologies.
   * non-lossy technological space travel
   * better support for non-functional properties
   * teach abstraction, shaping abstraction, modeling. Abstraction as an activity.
   * building libraries and APIs with reusability as a starting point
   * doing SLE earlier makes more students interested in PL
   * language prototyping: core of SLE teaches people making abstractions
   
* Discussion what should we teach before SLE is taught?
   * compiler construction
   * operational semantics
   * type systems

* Ralf proposes the subliminal SLE by just giving the students the tools and asking them to build something.

* Jurgen: There is the requirements and design perspective. The DDD perspective and modeling tools. Can we hook this all in? Mark says that DSL design is only after the requirements elicitation and the domain modeling. We have to link these things together. Ulrik agrees but the language the students design are lacking the proper abstractions. 

* It's a bridge too far to teach language design? No says Ralf. If you evaluate how students are using the tools then you can see their progress. Anya says the students make usable languages sometimes using language workbenches, but maybe API is a better way of teaching how to design abstractions.

* Tony: not every student is the same and also in time requirements for students  evolve. How do you generalize from a language if you haven't seen one from the inside? Ulrik says you can do simpler languages (domain specific). Eric says you should start with Scheme or Smalltalk.

* Ralf: what material do you use to teach language design? Martin Erweg's paper (? which one), and "Cognitive Dimensions". Fowler's DSL book (language implementation patterns) and Terence Parr's book.

* Massimo: this is bigger than SLE!

* Jaakko: there is a distinction between how language work and how to design languages.

* Thomas Kuhn: where do you cross the border between language design and using tools to build languages. Will the tools be there when the students have graduated? No!
   * Tony teaches attribute grammars and stuff from a conceptual level and provides the tools to practise with them.
   * Eric says the same. Don't teach Java, teach them OO and then use Java in the lab.
   * Ralf says the same: we use labs to exercise different kinds of technologies in the same classroom.
   
   
### 14:06

_The Moldable Debugger: a Framework for Developing Domain-Specific Debuggers, A. Chis, T. Girba and O. Nierstrasz_

I dropped into the _best student paper_ talk by Andrei Chis. Andrei demonstrates the actions a programmer takes when doing deduction and abduction steps while browsing the code in an advanced IDE. Like a good debugger he makes the decision steps, choices and the stack of reasoning explicit while clicking in the IDE and reading the information the debugger provides. Conclusion: debugging is repetitive and confusion for framework code (let's say an even handler).

The solution is to have a debugging perspective which is specialized for the framework. In this case an event framework. The contribution of the paper lies in the rapid prototyping/engineering of such debuggers. It can be applied to any domain, even very complex ones such as parsing frameworks.

The contribution of this paper lies at the core of SLE:
   * It helps software engineers solve complex daily problems
   * It takes the language perspective on API/frameworks
   * It generates IDE tools from higher level descriptions/API
   
We want more!

### 14:30

Now Magdalena Widl on the _best paper of SLE_: _A SAT-based Debugging Tool for State Machines and Sequence Diagrams, P. Kaufmann, M. Kronegger, A. Pfandler, M. Seidl, M. Widl_

Starting point: sequence diagrams show scenarios of state machines running (badly or not)

Goal: check whether a sequence diagram is consistent with a set of state machines? So this is a lighweight version of a model checking problem. But the problem is how to map state machines to the input languages to model checkers, so we mapped it directly to SAT. 

Héj, this is the first greek letters I am seeing at SLE this year :-) We are getting a short brain-refresh on propositional logic and satisfiability.

The encoding of sequence diagrams and state machines to propositional formulas works quite nicely. It shows how skipping a generic intermediate formalism in the middle can sometimes make things a lot easier. Normally we think that by standing on a plateau of some reusable language or framework gives benefit, but here we have evidence to the contrary. The generic model checking API/languages have an impedance mismatch with the kinds of sequence diagrams and state machines that Magdalena wants to model. It is easier to think of a mapping to logical variables and conjunctions then it is to find the mapping to the intermediate language.

Propositional logic is a great language.

Now this paper also uses random testing to evaluate the efficiency and the correctness of the implementation. Reporting on a thorough testing effort is a great way for SLE papers to evaluate and validate the claims.

### 15:04

Sebastian Gabmeyer presents: _Model Checking of CTL-Extended OCL Specifications, S. Gabmeyer, R. Bill, M. Seidl, P. Kaufmann_

* Starting point: we need automatic bug hunting tools because we have more and more software and it runs faster and faster. You can't keep up "manually".
* Technological space: EMF, Graph Transformations, OCL.
* Running example: the mission-critical software system: pacman
* Problem: check liveness and safety properties
* Solution: CTL-based model checking
* Enabler: extending OCL with CTL semantics: cOCL.

This looks good. I have some trouble positioning the work to general CTL-based model checking literature. One thing I believe is essential: the inclusion of CTL in the OCL language such that it is readily available in the OCL and Eclipse context. 

I found the explanation at the end a bit too detailed, because we lost the story line a bit there. What we have here is cOCL (OCL + CTL) and a model checker  (MocOCL) for this new language. A solid contribution, also from the engineering perspective.

You can try it at http://modelevolution.org/mococl 

### 16:02 

Finally: the tools sessions

First up: Tony Sloane on _"Monto: A Disintegrated Development Environment"_

First impression: it's like a modernized ToolBus of the Meta-Environment with JSON instead of ATerms and Python instead of T-script. Tony nicely mentioned ToolBus in his presentation btw. 

What we have is a truly simplified interaction model which allows one to quickly prototype an IDE-like experience. Quite cool, and all together in 146+32+17+34+10+9+62+35+43+57+4+5+309 = 763 lines of code.

### 16:28 

Next up is Ralf Lämmel demoing _"Test-data generation for Xtext with Xtextgen"_.

This is all about grammar-based testing. The result of a class Ralf taught about this topic.

Essential elements:
   * incrementally constraining the test data generator to generate more interesting sequences
   * post-processing to implement semantic constraints on the resulting 
   * extended by a grammar customization step where we rewrite the grammar to generate fewer sentences. Elegant and reminiscent of the grammar transformation operators of Vadim Zaytsev, Ralf and Jan Kort.
   
Ralf is lecturing sentence generation actually. Explaining it to us clearly. If you know the kind of elegant yet incomprehensible and also incompressible Prolog code that Ralf has written to generate sentences from grammars with specfic coverage criteria, you have to appreciate how he manages to tell the story today clearly.

And Ralf now shows a screencast of how to use the tool and generate input and he explains at the end how this work came about: out of an SLE course!

### 17:05

The final talk, _sniff_, of SLE 2014 is presented by Saverio: _"AIOCJ: A Choreographic Framework for Safe Adaptive Distributed Applications, M. D. Preda, M. Gabbrielli, S. Giallorenzo, I. Lanese, J. Maurio"_

Saverio is motivating high-level modeling of system coordination, i.e. separation of computation from coordinational protocol. 

The starting question is: dynamic update of the communication protocol, to get a safely adaptable distributed system. 






   










   
   






   





   

