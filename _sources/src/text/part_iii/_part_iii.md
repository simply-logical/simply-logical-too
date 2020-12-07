<!--H1: Part III-->
(part:iii)=
# Advanced reasoning techniques #

In {numref}`Part %s<part:i>`, we introduced the formalism of clausal logic and showed how it can be used in practice to perform logical inferences. In {numref}`Part %s<part:ii>`, we discussed the basic issues one encounters when writing a program to solve some reasoning task: how to represent the knowledge needed to solve the task, and how to search the space of possible solutions. In {numref}`Part %s<part:iii>`, we will go beyond the power of clausal logic in a number of ways.
<!--Part I Part II Part III-->

+++

<!--section 2.5-->
Why would one want to have a formalism more powerful than first-order clausal logic? One reason could be that we want to perform inferences that are simply not expressible in first-order clausal logic. We might want to express knowledge such as 'he inherited all his father's bad characteristics', which is a second-order statement ({numref}`sec:2.5`). We might want to express statements like 'Peter believes his boss knows he is writing a book', where 'Peter's boss knows' is a *modality* of the formula 'Peter is writing a book', and 'Peter believes' is a modality of the formula 'Peter's boss knows Peter is writing a book'. We might want to reason about sequences of events happening over time. Each of these examples requires a specialised logic extending the syntax of first-order logic. Needless to say, this increased expressiveness also requires more powerful semantics and proof theory.

+++

There are also reasoning tasks which use the language of clausal logic, but differ nonetheless from standard clausal logic in the validity of the conclusions drawn. For instance, the truth of a conclusion might not be guaranteed but only plausible, given the premises. Alternatively, a conclusion might be a general theory derived from a number of specific observations, a theory which might be falsified by new contradicting evidence. Typically, such non-standard reasoning tasks require a more elaborate semantic and proof-theoretic characterisation than required for standard logical inference.

+++

Thirdly, the knowledge required for the reasoning task might be available in non-logical form only: think of pictures, spoken or written text, or video images. In such cases, the reasoning task requires pre- and post-processing stages, in which the non-logical data are converted to and from logical formulas.

+++

In the following three chapters, we will encounter each of these three types of reasoning. {numref}`Chapter %s<ch:7>` is devoted to reasoning with knowledge expressed in natural language. We demonstrate how to translate sentences like 'Socrates is human' and 'all humans are mortal', and questions like 'is Socrates mortal?' into clausal logic, and how to obtain a natural language sentence as the answer. In {numref}`Chapter %s<ch:8>`, we discuss a number of approaches to reasoning with incomplete information. Most of these approaches are of the second type, extending semantics and proof theory but not syntax of clausal logic; one approach extends syntax as well. We provide a detailed discussion of how these approaches are related. Finally, inductive reasoning is discussed in {numref}`Chapter %s<ch:9>`. Induction aims at completing partial knowledge about specific instances of a theory, and is therefore, although related to, much harder than the forms of reasoning with incomplete knowledge discussed in {numref}`Chapter %s<ch:8>`. We give an in-depth analysis of the problem, and develop two Prolog programs that can inductively infer simple predicate definitions from examples.
<!--Chapter 7 Chapter 8 Chapter 9 Chapter 8-->
