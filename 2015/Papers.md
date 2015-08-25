---
layout: default2015
title: Accepted Papers
published: true
---

# SLE 2015 Accepted Papers

*(In presentation order.)*

## Language Development and Evaluation
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

## Formal Modeling and Language Validation
* Thomas Kühn, Stephan Böhme, [Sebastian
Götz](http://www.inf.tu-dresden.de/~sebgoetz) and [Uwe
Assmann](http://st.inf.tu-dresden.de/). *A Combined Formal Model for
Relational Context-Dependent Roles*

    Role-based modeling has been investigated for over 35 years as a promising paradigm to model complex, dynamic systems. Although current software systems are characterized by increasing complexity and context-dependence, all this research had almost no influence on current software development practice, still being discussed in recent literature. One reason for this is the lack of a coherent, comprehensive, readily applicable notion of roles. Researchers focused either on relational roles or context-dependent roles rather then combining both natures. Currently, there is no role-based modeling language sufficiently incorporating both the relational and context-dependent nature of roles together with the various proposed constraints. Hence, this paper formalizes a full-fledged role-based modeling language supporting both natures. To show its sufficiency and adequacy, a real world example is employed.
    
* Jesús J. López-Fernández, Esther Guerra and Juan de Lara. *Example-based
Validation of Domain-Specific Visual Languages*

    The definition of Domain-Specific Languages (DSLs) is a recurrent activity in Model-Driven Engineering. However, their construction is many times an ad-hoc process, partly due to the lack of tools for a proper engineering of DSLs, which should enable domain experts to play an active role. 

    In this paper, our focus is on the validation of meta-models for visual DSLs. For this purpose, we propose a language and tool support for describing properties that instances of meta-models should meet. Then, our system uses a model finder to produce example models, enriched with a graphical concrete syntax, that confirm or refute the assumptions of the meta-model developer. 

    Our language complements metaBEST, a framework for the validation and verification of meta-models that includes two other languages for unit testing and 
specification-based testing of meta-models. 

    A salient feature of our approach is that it fosters interaction with domain experts by the use, processing and creation of informal drawings constructed in editors liked yED or Dia. We assess the usefulness of the approach in the validation of a DSL for house blueprints, with the participation of 26 4th year computer science undergraduate students.

* Christoff Bürger. *Reference Attribute Grammar Controlled Graph
Rewriting: Motivation & Overview*

    Reference attribute grammars are a well-known language engineering technique for the implementation of semantic analyses. Reference attributes provide declarative means to extend abstract syntax trees to graphs and analyse such graphs; they are well-suited to deduce and reason about abstract syntax graphs. Efficient attribute re-evaluation in case of abstract syntax graph changes and a systematic integration of attribute-based analyses with further rewrite- based transformations are open research problems however. 

    To solve these problems, I present a novel incremental syntax-directed compiler-compiler technique that seamlessly combines reference attribute grammars and graph rewriting. The presented technique not only permits incremental refer- ence attribute evaluation, but also the reuse of analyses to ease the specification of, and guide, rewrite-based transfor- mations. It enables efficient, mutually dependent, memoized analyses and transformations. 

    My main focus is to motivate and explain these techniques; their realisation is only sketched.
    
## Tools I
* [Patrick Neubauer](http://www.big.tuwien.ac.at/staff/pneubaue),
[Alexander Bergmayr](http://www.big.tuwien.ac.at/staff/abergmayr),
[Tanja Mayerhofer](http://www.big.tuwien.ac.at/staff/tmayerhofer),
[Javier Troya](http://www.big.tuwien.ac.at/staff/jtroya) and [Manuel
Wimmer](http://www.big.tuwien.ac.at/staff/mwimmer). *XMLText: From XML Schema to Xtext* (Tool paper)

* [Loïc Gammaitoni](http://loic.gammaitoni.free.fr), [Pierre
Kelsen](http://wwwen.uni.lu/recherche/fstc/laboratory_of_advanced_software_systems_lassy/members/pierre_kelsen)
and Christian Glodt. *Designing Languages using Lightning* (Tool paper)

* [Anya Helene Bagge](http://www.ii.uib.no/~anya/). *Analysis and
Transformation with the Nuthatch Tree-Walking Library* (Tool paper)

## Model and Program Transformation
* Amine Benelallam, [Abel
Gómez-Llana](http://www.emn.fr/z-info/atlanmod/index.php/User:Agomez),
Massimo Tisi and [Jordi Cabot](http://jordicabot.com). *Distributed
Model-to-Model Transformation with ATL on MapReduce*

* Gianni Rosa, [Alfonso Pierantonio](http://www.di.univaq.it/alfonso) and
Romina Eramo. *Managing Uncertainty in Bidirectional Model
Transformations*

* Nico Ritschel and Sebastian Erdweg. *Modular Capture Avoidance for
Program Transformations*

## Model Execution and Verification
* Florent Latombe, [Xavier Crégut](http://cregut.perso.enseeiht.fr),
Benoit Combemale, Julien De Antoni and Marc Pantel. *Weaving Concurrency
in eXecutable Domain-Specific Modeling Languages*

* [Erwan Bousse](http://people.irisa.fr/Erwan.Bousse/), Jonathan Corley,
[Benoit Combemale](http://www.combemale.fr/), Jeff Gray and Benoit
Baudry. *A Generative Approach for Rich Omniscient Model Debugging*

* Lina Ochoa Venegas, Oscar González Rojas and [Thomas
Thüm](https://www.tu-braunschweig.de/isf/team/thuem). *Using Decision
Rules for Solving Conflicts in Extended Feature Models*

## Tools II
* David Pearce. *The Whiley Rewrite Language (WyRL)* (Tool paper)

* Nicolas Laurent and Kim Mens. *Parsing Expression Grammars Made Practical* (Tool paper)











