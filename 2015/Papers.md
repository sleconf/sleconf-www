---
layout: default2015
title: Accepted Papers
published: true
---

# SLE 2015 Accepted Papers and Best Papers

## Award Winners SLE 2015

##### Distinguished Research Paper Award

  * **Romina Eramo, Alfonso Pierantonio and Gianni Rosa**. *Managing Uncertainty in Bidirectional Model
Transformations*

##### Distinguished Tool Paper Award

  * **Anya Helene Bagge**. *Analysis and Transformation with the Nuthatch Tree-Walking Library*

##### Best Reviewer Award

  * **Zhenjiang Hu**

##### Best Presentation Award

  * **Sebastian Erdweg**. *Modular Capture Avoidance for
Program Transformations* (paper with Nico Ritschel)

## Papers
All papers are available in the [online proceedings at the ACM Digital Library](http://dl.acm.org/citation.cfm?id=2814251).

*(In presentation order.)*

## Language Development and Evaluation
*(Monday 26 Oct 2015 10:30–12:00)*

* Salome Maro, Matthias Tichy, Lars Gelin, Jan-Philipp Steghöfer and
Anthony Anjorin. **On Integrating Graphical and Textual Editors for a
UML-based Domain Specific Language**

    Domain Specific Languages (DSLs) are an established means of reducing the gap between problem and solution domains. DSLs increase productivity and improve quality as they can be tailored to exactly fit the needs of the problem to be solved. A DSL can have multiple types of notations, such as a textual notation or a graphical notation. In some cases, one of these notations for a DSL is enough but there are many cases where one notation does not suffice and there is a demand to support multiple notations for the same DSL. UML Profile, is one of the several approaches that one can use to define a DSL, however most UML tools only come with graphical editors. In this paper, we present our approach and industrial experience on integrating textual and graphical editors for a UML based DSL. This work was conducted as part of an explorative study at Ericsson. The main aim of the study was to find out how to introduce a textual editor to an already existing UML based DSL in an Eclipse environment. We report on the challenges of integrating textual and graphical editors in practice, our chosen approach, specific constraints and requirements of the case study.

* Eric Umuhoza, [Marco Brambilla](http://home.dei.polimi.it/mbrambil/),
[Jordi Cabot](http://jordicabot.com) and Davide Ripamonti. **An Empirical
Study on Simplification of Business Process Modeling Languages**

    The adaptation, specially by means of a simplification process, of modeling languages is a common practice due to the overwhelming complexity of most standard languages (like UML or BPMN), not needed for typical usage scenarios while at the same time companies don’t want to go to the extreme of defining a brand new domain specific language. Unfortunately, there is a lack of examples of such simplification experiences that can be used as a reference for future projects. 

    In this paper we report on a field study aimed at the simplification of a business process modeling language (namely, BPMN) for making it suitable to end users. Our simplification process relies on a set of steps that encompass the selection of the language elements to simplify, generation of a set of language variants for those elements, measurement of effectiveness of the variants through modeling sessions performed by intended users, and extraction of quantitative and qualitative data for guiding the selection of the best language refinement. We describe the experimental setting, the output of the various steps of the analysis, and the results we obtained from users. Finally, we conclude with an outlook towards the generalization of the approach and consolidation of a language simplification method. 

* [Thomas Degueule](http://people.irisa.fr/Thomas.Degueule/), [Benoit
Combemale](http://www.combemale.fr/), [Arnaud
Blouin](http://people.irisa.fr/Arnaud.Blouin/), [Olivier
Barais](http://olivier.barais.fr) and [Jean-Marc
Jézéquel](http://www.irisa.fr/prive/jezequel). **Melange: a meta-language
for modular and reusable development of DSLs**

    Domain-Specific Languages (DSLs) are now developed for a wide variety of domains to address specific concerns in the development of complex systems. When engineering new DSLs, it is likely that previous efforts spent on the development of other languages could be leveraged, especially when their domains overlap. However, legacy DSLs may not fit exactly the end user requirements and thus require further extension, restriction, or specialization. While current language workbenches provide import mechanisms, they usually lack an explicit support for such customizations of imported artifacts. In this paper, we propose an approach for building DSLs by safely assembling and customizing legacy DSLs artifacts. This approach is based on a dedicated type system that provides a reasoning layer for manipulating DSLs while ensuring type safety. On top of this type system, we provide an algebra of operators for extending, restricting, and assembling separate DSL artifacts. We implemented the type system and algebra into the Melange meta-language. We illustrate Melange through the modular definition of an executable modeling language for the Internet Of Things domain. We show how it eases the definition of new DSLs by maximizing the reuse of legacy artifacts without introducing issues in terms of performance, technical ecosystem compatibility, or generated code volume.

## Model and Program Transformation
*(Monday 26 Oct 2015 13:30–15:00)*

* Amine Benelallam, [Abel
Gómez-Llana](http://www.emn.fr/z-info/atlanmod/index.php/User:Agomez),
Massimo Tisi and [Jordi Cabot](http://jordicabot.com). **Distributed
Model-to-Model Transformation with ATL on MapReduce**

    Efficient processing of very large models is a key requirement for the adoption of Model-Driven Engineering (MDE) in some industrial contexts. One of the central operations in MDE is rule-based model transformation (MT). It is used to specify manipulation operations over structured data coming in the form of model graph. However, being based on computationally expensive operations like subgraph isomorphism, MT tools are facing issues on both memory occupancy and execution time while dealing with the increasing model size and complexity. One way to overcome these issues is to exploit the wide availability of distributed clusters in the Cloud for the distributed execution of MT.

    In this paper, we propose an approach to automatically distribute the execution of model transformations written in a popular MT language, ATL, on top of a well-known distributed programming model, MapReduce. We show how the execution semantics of ATL can be aligned with the MapReduce computation model. We describe the extensions to the ATL transformation engine to enable distribution, and we experimentally demonstrate the scalability of this solution in a reverse-engineering scenario.


* Romina Eramo, [Alfonso Pierantonio](http://www.di.univaq.it/alfonso) and Gianni Rosa. **Managing Uncertainty in Bidirectional Model Transformations**

    **Distinguished Research Paper Award**
    
    In Model-Driven Engineering bidirectionality in transformations is regarded as a key mechanism. Recent approaches to non-deterministic transformations have been proposed for dealing with non-bijectivity. Among them, the JTL language is based on a relational model transformation engine which restores consistency by returning all admissible models. This can be regarded as an uncertainty reducing process: the unknown uncertainty at design-time is translated into known uncertainty at run-time by generating multiple choices. Unfortunately, little changes in a model usually correspond to a combinatorial explosion of the solution space. This paper proposes to represent the multiple solutions in a intensional manner by adopting a model for uncertainty. The technique is applied to JTL demonstrating the advantages of the proposal.

* Nico Ritschel and Sebastian Erdweg. **Modular Capture Avoidance for
Program Transformations**

    **Best Presentation Award**
    
    The application of program transformations and refactorings involves the risk of capturing variables, which may break the intended semantics of the transformed code. One way to resolve variable capture is by renaming of the involved identifiers. However, in a modular context, the renaming of exported declarations is undesirable (affecting a module's clients), and the renaming of imported declarations is impossible (requiring changes to third-party modules).

    We present an algorithm name-fix that detects and eliminates variable capture modularly. We extend a previous non-modular version of name-fix in order to (i) minimize renamings of exported declarations, (ii) propagate necessary renamings of exported declarations to clients, and (iii) avoid renamings of imported declarations altogether. Together with support for transitive name bindings and conflicting declarations, our extensions to name-fix enable the application to real-world languages that feature separate compilation. To demonstrate the applicability of name-fix, we use it to modularly resolve variable capture for optimizations, refactorings, and desugarings of Lightweight Java.


## Tools I
*(Monday 26 Oct 2015 15:30–17:00)*

* [Patrick Neubauer](http://www.big.tuwien.ac.at/staff/pneubaue), [Alexander Bergmayr](http://www.big.tuwien.ac.at/staff/abergmayr), [Tanja Mayerhofer](http://www.big.tuwien.ac.at/staff/tmayerhofer), [Javier Troya](http://www.big.tuwien.ac.at/staff/jtroya) and [Manuel Wimmer](http://www.big.tuwien.ac.at/staff/mwimmer). **XMLText: From XML Schema to Xtext** (Tool paper)

    A multitude of Domain-Specific Languages (DSLs) have been implemented with XML Schemas. While such DSLs are well adopted and flexible, they miss modern DSL editor functionality. Moreover, since XML is primarily designed as a machine-processible format, artifacts defined with XML-based DSLs lack comprehensibility and, therefore, maintainability.
    In order to tackle these shortcomings, we propose a bridge between the XML Schema Definition (XSD) language and text-based metamodeling languages. This bridge exploits existing seams between these two worlds and closes identified gaps. The resulting approach is able to generate Xtext-based editors from XSDs providing powerful editor functionality, customization options for the textual concrete syntax style, and round-trip transformations enabling the exchange of data between these two worlds.
    We evaluate our approach by a case study on TOSCA, which is an XML-based standard for defining Cloud deployments. The results show that our approach enables bridging XMLware with modelware and grammarware in several ways going beyond existing approaches and allows the automated generation of editors that are at least equivalent to editors manually built for XML-based languages.

* [Loïc Gammaitoni](http://loic.gammaitoni.free.fr), [Pierre
Kelsen](http://wwwen.uni.lu/recherche/fstc/laboratory_of_advanced_software_systems_lassy/members/pierre_kelsen)
and Christian Glodt. **Designing Languages using Lightning** (Tool paper)

    Modelling languages are defined by specifying their abstract syntax, concrete syntax and semantics. In the Lightning tool the definition of all these language components is based on the lightweight formal language Alloy. Lightning makes use of the powerful automatic analysis features of Alloy to allow language designers to develop and validate the definition of a modelling language in an incremental fashion. By providing immediate visual feedback, it allows errors in the language definition to be quickly identified and corrected. Furthermore Lightning introduces a novel interpretation mechanism that allows efficient execution of transformations used in the language definition. We illustrate the use of the tool on the language of structured business processes.


* [Anya Helene Bagge](http://www.ii.uib.no/~anya/). **Analysis and
Transformation with the Nuthatch Tree-Walking Library** (Tool paper)

    **Distinguished Tool Paper Award**
    
    Nuthatch is a system for traversing, collecting information from, and  rewriting trees, based on the idea of tree walking. The main application  is software analysis and transformation. Nuthatch traversals are  non-recursive by default and independent of the concrete tree  representation. We provide an extensible library, Nuthatch/J, for doing  tree walking in Java, with adapters for interfacing with popular software  transformation tools like Stratego/XT and Rascal.  

    Transformations are described as walks that proceed in programmer-defined  steps. Each step can perform actions based on observed properties of  current node and walk, and affect state associated with the walk and also  rewrite the walked tree. A step ends by walking to a different node in  the tree, following the tree branches, and the walk ends by returning to  the top.

## Keynote
*(Tuesday 27 Oct 2015 08:30–10:00)*

*  Stephane Ducasse. **What's the value of an end user? Platforms and Research: The case of Pharo and Moose**

    This talk will present the synergy arising from building platforms on top of which do our research. [RMOD our team](http://rmod.lille.inria.fr/) is developing two platforms: Pharo (a dynamic reflective object-oriented language supporting live programming) and [Moose](http://www.moosetechnology.org/) (an open-source software analysis platform). Developing platforms forces us to develop really usable systems. While some activities are more engineering than research per se, it is really interesting to deeply understand problems or impacts of certain design decisions. Developing platforms is rewarding because it is more a long term effort and ensures a degree of stability. Platforms also often exhibit non-linear growth that is really exciting. Finally this setup raises many interesting questions such as “What is the value in terms of citations or published papers of a couple of end-users”, or “Is it not really stupid not to work on latest hype language?” To try to open our minds, I will draw parallels with the notion of wealth of an ecosystem in biology. In the second part of the talk I will present some selected results around Pharo and Moose such as: automatic minimal system core generation, dynamic core updates, selector namespace, dependencies in past commit branches and automatic migration rule generation.
    

## Formal Modeling and Language Validation
*(Tuesday 27 Oct 2015 10:30–12:00)*

* Thomas Kühn, Stephan Böhme, [Sebastian
Götz](http://www.inf.tu-dresden.de/~sebgoetz) and [Uwe
Assmann](http://st.inf.tu-dresden.de/). **A Combined Formal Model for
Relational Context-Dependent Roles**

    Role-based modeling has been investigated for over 35 years as a promising paradigm to model complex, dynamic systems. Although current software systems are characterized by increasing complexity and context-dependence, all this research had almost no influence on current software development practice, still being discussed in recent literature. One reason for this is the lack of a coherent, comprehensive, readily applicable notion of roles. Researchers focused either on relational roles or context-dependent roles rather then combining both natures. Currently, there is no role-based modeling language sufficiently incorporating both the relational and context-dependent nature of roles together with the various proposed constraints. Hence, this paper formalizes a full-fledged role-based modeling language supporting both natures. To show its sufficiency and adequacy, a real world example is employed.
    
* Jesús J. López-Fernández, Esther Guerra and Juan de Lara. **Example-based
Validation of Domain-Specific Visual Languages**

    The definition of Domain-Specific Languages (DSLs) is a recurrent activity in Model-Driven Engineering. However, their construction is many times an ad-hoc process, partly due to the lack of tools for a proper engineering of DSLs, which should enable domain experts to play an active role. 

    In this paper, our focus is on the validation of meta-models for visual DSLs. For this purpose, we propose a language and tool support for describing properties that instances of meta-models should meet. Then, our system uses a model finder to produce example models, enriched with a graphical concrete syntax, that confirm or refute the assumptions of the meta-model developer. 

    Our language complements metaBEST, a framework for the validation and verification of meta-models that includes two other languages for unit testing and 
specification-based testing of meta-models. 

    A salient feature of our approach is that it fosters interaction with domain experts by the use, processing and creation of informal drawings constructed in editors liked yED or Dia. We assess the usefulness of the approach in the validation of a DSL for house blueprints, with the participation of 26 4th year computer science undergraduate students.

* Christoff Bürger. **Reference Attribute Grammar Controlled Graph
Rewriting: Motivation & Overview**

    Reference attribute grammars are a well-known language engineering technique for the implementation of semantic analyses. Reference attributes provide declarative means to extend abstract syntax trees to graphs and analyse such graphs; they are well-suited to deduce and reason about abstract syntax graphs. Efficient attribute re-evaluation in case of abstract syntax graph changes and a systematic integration of attribute-based analyses with further rewrite- based transformations are open research problems however. 

    To solve these problems, I present a novel incremental syntax-directed compiler-compiler technique that seamlessly combines reference attribute grammars and graph rewriting. The presented technique not only permits incremental refer- ence attribute evaluation, but also the reuse of analyses to ease the specification of, and guide, rewrite-based transfor- mations. It enables efficient, mutually dependent, memoized analyses and transformations. 

    My main focus is to motivate and explain these techniques; their realisation is only sketched.
 

## Model Execution and Verification
*(Tuesday 27 Oct 2015 13:30–15:00)*

* Florent Latombe, [Xavier Crégut](http://cregut.perso.enseeiht.fr),
Benoit Combemale, Julien De Antoni and Marc Pantel. **Weaving Concurrency
in eXecutable Domain-Specific Modeling Languages**

    The emergence of modern concurrent systems (e.g., Cyber-Physical Systems or the Internet of Things) and highly-parallel platforms (e.g., many-core, GPGPU and distributed platforms) calls for Domain-Specific Modeling Languages (DSMLs) where concurrency is of paramount importance. Such DSMLs are intended to propose constructs with rich concurrency semantics, which allow system designers to precisely define and analyze system behaviors. However, specifying and implementing the execution semantics of such DSMLs can be a difficult, costly and error-prone task. Most of the time the concurrency model remains implicit and ad-hoc, embedded in the underlying execution environment. The lack of an explicit concurrency model prevents: the precise definition, the variation and the complete understanding of the DSML's semantics, the effective usage of concurrency-aware analysis techniques, and the exploitation of the concurrency model during the system refinement (e.g., during its allocation on a specific platform). In this paper, we introduce a concurrent executable metamodeling approach, which supports a modular definition of the execution semantics, including the concurrency model, the semantic rules, and a well-defined and expressive communication protocol between them. This protocol supports both the mapping of the concurrency model to the semantic rules, and the feedback, possibly with data, from the semantic rules to the concurrency model. Our approach comes with a dedicated meta-language to specify the communication protocol, and with an execution environment to simulate executable models. We illustrate and validate our approach with an implementation of fUML, and discuss the modularity and applicability of our approach.

* [Erwan Bousse](http://people.irisa.fr/Erwan.Bousse/), Jonathan Corley,
[Benoit Combemale](http://www.combemale.fr/), Jeff Gray and Benoit
Baudry. **Supporting Efficient and Advanced Omniscient Debugging for xDSMLs**

    Omniscient debugging is a promising technique that relies on execution traces to enable free traversal of the states reached by a system during an execution. While some General-Purpose Languages (GPLs) already have support for omniscient debugging, developing such a complex tool for any executable Domain-Specific Modeling Language (xDSML) remains a challenging and error prone task. A solution to this problem is to define a generic omniscient debugger for all xDSMLs. However, generically supporting any xDSML both compromises the efficiency and the usability of such an approach. Our contribution relies on a partly generic omniscient debugger supported by generated domain-specific trace management facilities. Being domain-specific, these facilities are tuned to the considered xDSML for better efficiency. Usability is strengthened by providing multidimensional omniscient debugging. Results show that our approach is on average 3.0 times more efficient in memory and 5.03 more efficient in time when compared to a generic solution that copies the model at each step.

* Lina Ochoa Venegas, Oscar González Rojas and [Thomas
Thüm](https://www.tu-braunschweig.de/isf/team/thuem). **Using Decision
Rules for Solving Conflicts in Extended Feature Models**

    Software Product Line Engineering has introduced feature modeling as a domain analysis technique used to represent the variability of software products and decision-making scenarios. We present a model-based transformation approach to solve conflicts among configurations performed by different stakeholders on feature models. We propose the usage of a domain-specific language named CoCo to specify attributes as non-functional properties of features, and to describe business-related decision rules in terms of costs, time, and human resources. These specifications along with the stakeholders' configurations and the feature model are transformed into a constraint programming problem, on which decision rules are executed to find a non-conflicting set of solution configurations that are aligned to business objectives. We evaluate CoCo compositionality and model complexity simplification while using a set of motivating decision scenarios.


## Tools II and Closing
*(Tuesday 27 Oct 2015 15:30–17:00)*

* David Pearce. **The Whiley Rewrite Language (WyRL)** (Tool paper)

    The Whiley Rewrite Language (WyRL) is a standalone tool providing a domain-specific declarative rewrite language and code generator. The tool is currently used to generate a critical component of the Whiley verifying Compiler, namely the automated theorem prover. The tool automatically generates Java source code from a given rule set. The runtime library provides support for different heuristics to control aspects of the generated system, such as the order in which rewrite rules are applied.

    Although WyRL was originally designed specifically for use with the Whiley compiler, it has application outside this. For example, one can easily develop the core component of a type checker for a wide range of type systems, particularly those involving recursive types. In this tool presentation, I will demonstrate the tool being used to construct a range of different systems, including type systems, simple constraint solvers and a deductive verification system for propositional logic. Furthermore, I will discuss some of the issues faced in generating a full-featured SMT solver using declarative rewrite rules.

* Nicolas Laurent and Kim Mens. **Parsing Expression Grammars Made Practical** (Tool paper)

    Parsing Expression Grammars (PEGs) define languages by specifying a recursive-descent parser that recognises them. The PEG formalism exhibits desirable properties, such as closure under composition, built-in disambiguation, unification of syntactic and lexical concerns, and closely matching programmer intuition. Unfortunately, state of the art PEG parsers struggle with left-recursive grammar rules, which are not supported by the original definition of the formalism and can lead to infinite recursion under naive implementations. Likewise, support for associativity and explicit precedence is spotty. To remedy these issues, we introduce Autumn, a new general purpose PEG library that supports left-recursion, left and right associativity and precedence rules, and does so efficiently. Furthermore, we identify infix and postfix expressions as a major source of inefficiency in left-recursive PEG parsers and show how to tackle this problem. We also explore the modular nature of PEG grammars by showing how one can easily introduce new parsing operators and how our parser accommodates custom memoization and error handling strategies. We compare our parser to both state of the art and battle-tested PEG and CFG parsers, such as Rats!, Parboiled and ANTLR.









