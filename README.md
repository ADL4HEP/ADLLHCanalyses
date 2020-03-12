# ADLLHCanalyses
ADL implementations of LHC analyses
this is not added to CutLang git repository as a submodule

ADL (for Analysis Description Language) [1,2] is a recently developed domain-specific language for describing event selections.In ADL, analyses are written in plain text files separating object, variable and event selection definitions in blocks following a keyword-value structure, where keywords specify analysis concepts and operations. ADL syntax includes mathematical and logical operations, comparison and optimisation operators, reducers, four-vector algebra and common HEP-specific functions (e.g. d\phi, dR).  ADL files can be complemented by and can refer to self-contained functions encapsulating variables with complex algorithms (e.g. M_T2, aplanarity) or non-analytic variables (e.g. efficiency tables, machine learning discriminators). 

There are currently two interpreters that parse and run analyses written in ADL: __adl2tnm__ [3] and __cutlang__ [4,5].
__adl2tnm__ is a Python transpiler that converts an analysis written in ADL into a complete C++ analysis code. __cutlang__ is a runtime interpreter that directly runs an analysis written in ADL on events without the need for compilation. Both frameworks can process a variety of event formats and be used for experimental analysis or phenomenology studies. 

References:

[1] http://arxiv.org/abs/1605.02684

[2] http://arxiv.org/abs/2002.12220

[3] http://arxiv.org/abs/1803.10379

[4] http://arxiv.org/abs/1801.05727

[5] http://arxiv.org/abs/1909.10621
