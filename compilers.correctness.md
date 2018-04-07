# [C++ links](README.md): compilers - correctness

Note: see also [compilers](compilers.md)

# Contents

* [General](#general)
* [Testing](#testing)
	+ [Articles](#articles)
	+ [Software](#software)
	+ [Talks](#talks)
* [Validation](#validation)
* [Verification](#verification)

---

# General

* ACM SIGPLAN Conference on Certified Programs and Proofs (CPP) - http://dblp.org/db/conf/cpp/
* How to prove a compiler correct - Daniel Patterson
	+ https://dbp.io/essays/2018-01-16-how-to-prove-a-compiler-correct.html
	+ https://github.com/dbp/howtoproveacompiler
* What even is compiler correctness? - https://www.williamjbowman.com/blog/2017/03/24/what-even-is-compiler-correctness/

# Testing

* Dagstuhl Seminar 17502 – Testing and Verification of Compilers
	+ December 2017
	+ http://dagstuhl.de/17502
	+ Materials: http://materials.dagstuhl.de/index.php?semnr=17502
* EMI-based Compiler Testing - http://web.cs.ucdavis.edu/~su/emi-project/

## Articles

* An empirical comparison of compiler testing techniques
	+ International Conference on Software Engineering (ICSE 2016)
	+ Junjie Chen, Wenxiang Hu, Dan Hao, Yingfei Xiong, Hongyu Zhang, Lu Zhang, Bing Xie
	+ http://sei.pku.edu.cn/~xiongyf04/papers/ICSE16.pdf
	+ http://emponcc.github.io/
	+ https://github.com/emponcc/emponcc.github.io/blob/master/CompilerTestingComparison.md
	+ https://dl.acm.org/citation.cfm?id=2884878
* Automatic Test Case Reduction for OpenCL - https://dl.acm.org/citation.cfm?id=2909439
	+ paper: https://spiral.imperial.ac.uk/handle/10044/1/39576
	+ slides: http://www.iwocl.org/wp-content/uploads/iwocl-2016-automatic-test-case-reduction.pdf
* Automated Testing of Graphics Shader Compilers
	+ https://www.doc.ic.ac.uk/~afd/homepages/papers/pdfs/2017/OOPSLA.pdf
	+ Overview of the GLFuzz transformations - https://medium.com/@afd_icl/overview-of-the-glfuzz-transformations-d530540a5a18
* Automatic Testing of Symbolic Execution Engines via Program Generation and Differential Testing - https://srg.doc.ic.ac.uk/files/papers/symex-engine-tester-ase-17.pdf
* Checking Correctness of Code Generator Architecture Specifications 
	+ Code Generation and Optimization (CGO) 2015
	+ N. Hasabnis, R. Qiao, R. Sekar 
	+ http://www3.cs.stonybrook.edu/~nhasabni/papers/cgo15.pdf
	+ http://www3.cs.stonybrook.edu/~nhasabni/papers/cgo15_talk.pdf
* DATm: Diderot's Automated Testing Model.
	+ 39th International Conference on Software Engineering ICSE (12th International Workshop on Automation of Software Test AST) 2017
	+ C. Chiw, G. Kindlmann, J. Reppy
	+ https://www.researchgate.net/publication/317836930_DATm_Diderot%27s_Automated_Testing_Model
	+ https://www.dropbox.com/s/5twsrp12vg4or7t/datm_talk.key?dl=0
* Detecting Arithmetic Optimization Opportunities for C Compilers by Randomly Generated Equivalent Programs, IPSJ Transactions on System LSI Design Methodology, vol. 9, 2016. A. Hashimoto and N. Ishiura. <https://www.jstage.jst.go.jp/article/ipsjtsldm/9/0/9_21/_article>
* Detecting Missed Arithmetic Optimization in C Compilers by Differential Random Testing - http://ist.ksc.kwansei.ac.jp/~ishiura/publications/C2016-10a.pdf
* Differential Testing for Software - http://www.cs.dartmouth.edu/~mckeeman/references/DifferentialTestingForSoftware.pdf
* Effect-Driven QuickChecking of Compilers
	+ ICFP 2017
	+ Jan Midtgaard, Mathias Nygaard Justesen, Patrick Kasting, Flemming Nielson, Hanne Riis Nielson
	+ paper: http://janmidtgaard.dk/papers/Midtgaard-al%3AICFP17-full.pdf
	+ implementation: https://github.com/jmid/efftester
	+ talk
		- http://podcasts.ox.ac.uk/effect-driven-quickchecking-compilers
		- https://www.youtube.com/watch?v=_KrZzaShDew&list=PLnqUlCo055hW7kU-SBQEhC_87etA5Gqlq&index=15
* Evaluating the Effects of Compiler Optimizations on Mutation Testing at the Compiler IR Level - ISSRE’16
	+ http://mir.cs.illinois.edu/farah/presentations/issre16_presentation.pdf
	+ http://mir.cs.illinois.edu/marinov/publications/HaririETAL16CompilerIRMutation.pdf
	+ https://www.researchgate.net/publication/311529837_Evaluating_the_Effects_of_Compiler_Optimizations_on_Mutation_Testing_at_the_Compiler_IR_Level
* Finding and Analyzing Compiler Warning Defects - http://ieeexplore.ieee.org/document/7886904/
* Finding Missed Compiler Optimizations by Differential Testing
	+ Compiler Construction (CC) 2018
	+ Gergö Barany
	+ https://github.com/gergo-/missed-optimizations/raw/master/missed_optimizations_preprint.pdf
	+ Missed optimizations in C compilers: https://github.com/gergo-/missed-optimizations/
	+ https://hal.inria.fr/hal-01682683
* Finding and Understanding Bugs in C Compilers
	+ http://www.cs.utah.edu/~regehr/papers/pldi11-preprint.pdf
	+ https://www.flux.utah.edu/download?uid=114
	+ https://blog.regehr.org/archives/492
	+ http://lambda-the-ultimate.org/node/4241
* Learning to Prioritize Test Programs for Compiler Testing
	+ International Conference on Software Engineering (ICSE 2017)
	+ Junjie Chen, Yanwei Bai, Dan Hao, Yingfei Xiong, Hongyu Zhang, Bing Xie
	+ http://sei.pku.edu.cn/~xiongyf04/papers/ICSE17b.pdf
* RandIR: Differential Testing for Embedded Compilers - https://www.cs.purdue.edu/homes/rompf/papers/ofenbeck-scala16.pdf
* Reinforcing Random Testing of Arithmetic Optimization of C Compilers by Scaling up Size and Number of Expressions, IPSJ Transactions on System LSI Design Methodology, vol. 7, 2014. E. Nagai, A. Hashimoto, and N. Ishiura. <https://www.jstage.jst.go.jp/article/ipsjtsldm/7/0/7_91/_article>
* Scaling up Size and Number of Expressions in Random Testing of Arithmetic Optimization of C Compilers
	+ SASIMI 2013
	+ http://ist.ksc.kwansei.ac.jp/~ishiura/publications/C2013-10.pdf
* Some Goals for High-impact Verified Compiler Research - https://blog.regehr.org/archives/1565
* System Under Test: LLVM - https://systemundertest.org/llvm/
* Taming compiler fuzzers
	+ PLDI 2013
	+ Y. Chen, A. Groce, C. Zhang, W.-K. Wong, X. Fern, E. Eide, J. Regehr
	+ https://www.cs.utah.edu/~regehr/papers/pldi13.pdf
	+ Fuzzers Need Taming - https://blog.regehr.org/archives/925
* Test-Case Reduction for C Compiler Bugs - https://www.cs.utah.edu/~regehr/papers/pldi12-preprint.pdf
* Testing LLVM - http://blog.regehr.org/archives/1450
* The Correctness-Security Gap in Compiler Optimization - LangSec 2015, IEEE SPW
	+ paper: https://research.google.com/pubs/pub43856.html
	+ slides: https://nebelwelt.net/publications/files/15LangSec-presentation.pdf
	+ talk: https://www.youtube.com/watch?v=g6LCtHz_MDc&list=PL0pRF4xvoD0kuECJuowraVIIHlT3pN1Cm&index=3
* The problem with differential testing is that at least one of the compilers must get it right - http://blog.frama-c.com/index.php?post/2013/09/25/The-problem-with-differential-testing-is-that-at-least-one-of-the-compilers-must-get-it-right

## Software

* CF3: Test suite for arithmetic optimization of C compilers
	+ https://ist.ksc.kwansei.ac.jp/~ishiura/pub/CF3/
	+ https://github.com/ishiura-compiler/CF3
* Csmith, a random generator of C programs
	+ https://github.com/csmith-project/csmith
	+ https://embed.cs.utah.edu/csmith/
	+ Csmith testing - http://blog.frama-c.com/index.php?pages/Csmith-testing
* C-Reduce, a C program reducer
	+ https://embed.cs.utah.edu/creduce/
	+ https://github.com/csmith-project/creduce
* Fuzzing LLVM libraries and tools - https://llvm.org/docs/FuzzingLLVM.html
	+ Adventures in Fuzzing Instruction Selection
		- 2017 EuroLLVM Developers’ Meeting; Justin Bogner
		- http://llvm.org/devmtg/2017-03/assets/slides/adventures_in_fuzzing_instruction_selection.pdf
		- https://www.youtube.com/watch?v=UBbQ_s6hNgg
	+ Structure-aware fuzzing for Clang and LLVM with libprotobuf-mutator
		- 2017 LLVM Developers’ Meeting; Kostya Serebryany, Vitaly Buka, Matt Morehouse
		- https://www.youtube.com/watch?v=U60hC16HEDY
* kscope
	+ a library which recursively generates randomized code while keeping it 100% equivalent to the original one
	+ http://ithare.com/c17-compiler-bug-hunt-very-first-results-12-bugs-reported-3-already-fixed/
	+ https://github.com/ITHare/kscope
* ldrgen: Liveness-driven random C code generator - https://github.com/gergo-/ldrgen
* llvm-mutate – mutate LLVM IR - http://eschulte.github.io/llvm-mutate/
* opt-fuzz: a simple implementation of bounded exhaustive testing for LLVM programs
	+ https://github.com/regehr/opt-fuzz
* Orange3
	+ a tool to test C compilers with randomly generated programs; mainly targets arithmetic optimization such as constant folding.
	+ https://ist.ksc.kwansei.ac.jp/~ishiura/pub/orange3/
	+ https://github.com/ishiura-compiler/Orange3
* Orange4
	+ a tool to test C compilers by randomly generated programs; based on equivalent transformations on C programs and can generate wider class of C test programs than Orange3.
	+ https://ist.ksc.kwansei.ac.jp/~ishiura/pub/orange4/
	+ https://github.com/ishiura-compiler/Orange4
* prog-fuzz: Compiler/source code fuzzing tool using AFL instrumentation
	+ https://github.com/vegard/prog-fuzz
* Quest: A tool for testing C compilers - https://github.com/lindig/quest
* shader-compiler-bugs: A collection of shader compiler bugs - https://github.com/mc-imperial/shader-compiler-bugs
* yarpgen: Yet Another Random Program Generator
	+ a random C/C++ program generator, which produces correct runnable C/C++ programs
	+ specifically designed to trigger compiler optimization bugs and is intended for compiler testing
	+ https://github.com/intel/yarpgen

## Talks

* Coverage-Directed Differential Testing of JVM Implementations - Yuting Chen, PLDI 2016
	+ https://www.youtube.com/watch?v=2Reaqfp4v-g
	+ http://cse.sjtu.edu.cn/~zhao/pub/pdf/pldi2016.pdf
* 2017 EuroLLVM Developers’ Meeting: J. Bogner “Adventures in Fuzzing Instruction Selection”
	+ https://www.youtube.com/watch?v=UBbQ_s6hNgg
	+ http://llvm.org/devmtg/2017-03//assets/slides/adventures_in_fuzzing_instruction_selection.pdf
* Exposing Difficult Compiler Bugs With Random Testing
	+ https://gcc.gnu.org/wiki/summit2010?action=AttachFile&do=get&target=regehr_gcc_summit_2010.pdf
* Testing Language Implementations - Alastair Donaldson - Programming Language Implementation Summer School (PLISS) 2017
	+ https://www.youtube.com/watch?v=ZJUk8_k1HbY

# Validation

Validation: Including translation validation, equivalence checking.

* Black-box equivalence checking across compiler optimizations - APLAS ’17 (2017) - http://www.cse.iitd.ac.in/~sbansal/pubs/aplas17.pdf
* Modeling undefined behaviour semantics for checking equivalence across compiler optimizations - Manjeet Dahiya, Sorav Bansal. HVC 2017
	+ http://www.cse.iitd.ernet.in/~sbansal/pubs/hvc17.pdf
	+ http://www.cse.iitd.ac.in/~dahiya/hvc17.pdf
* Evaluating value-graph translation validation for LLVM
	+ Programming and Language Design Implementation (PLDI) 2011
	+ Tristan, Jean-Baptiste, Paul Govereau, Greg Morrisett
	+ https://dl.acm.org/citation.cfm?id=1993498.1993533
* Formally Verified Compilation of Low-Level C code
	+ 2016 PhD Dissertation; Pierre Wilke
	+ https://tel.archives-ouvertes.fr/tel-01483676
* Proving the correctness of heuristically optimized code
	+ Hanan Samet, CACM 1978
	+ http://www.cs.umd.edu/~hjs/pubs/compilers/proving-correctness.pdf
* Translation validation
	+ TACAS 1998
	+ Amir Pnueli, Michael Siegel, Eli Singerman
	+ https://dl.acm.org/citation.cfm?id=349314
	+ "We present the notion of _translation validation_ as a new approach to the verification of translators (compilers, code generators). Rather than proving in advance that the compiler always produces a target code which correctly implements the source code (compiler verification), each individual translation (i.e. a run of the compiler) is followed by a validation phase which verifies that the target code produced on this run correctly implements the submitted source program."
* Translation Validation: Automatically Proving the Correctness of Translations Involving Optimized Code
	+ [Hanan Samet](http://www.cs.umd.edu/~hjs/)
	+ translation validation - http://www.cs.umd.edu/~hjs/hjscat.html#sectiontranslationvalidation
	+ compiler testing - http://www.cs.umd.edu/~hjs/hjscat.html#sectioncompilertesting
	+ http://www.cs.umd.edu/~hjs/pubs/compilers/CS-TR-75-498.pdf
	+ http://www.cs.umd.edu/~hjs/slides/translation-validation-slides.pdf
* Translation Validation: From DC+ to C*
	+ FM-Trends 1998
	+ Amir Pnueli, Ofer Shtrichman, Michael Siegel
	+ https://dl.acm.org/citation.cfm?id=729871
	+ "Translation validation is an alternative to the verification of translators (compilers, code generators). Rather than proving in advance that the compiler always produces a target code which correctly implements the source code (compiler verification), each individual translation (i.e. a run of the compiler) is followed by a validation phase which verifies that the target code produced on this run correctly implements the submitted source program."
* Translation validation for an optimizing compiler
	+ PLDI 2000
	+ George C. Necula
	+ https://dl.acm.org/citation.cfm?id=349314
* Translation Validation of Bounded Exhaustive Test Cases - Nuno Lopes, John Regehr - https://blog.regehr.org/archives/1510
* Translation Validation with Alive - https://github.com/nunoplopes/alive/tree/newsema/tv

# Verification

* ALIVe: Automatic LLVM InstCombine Verifier
	+ https://github.com/nunoplopes/alive
	+ online: http://rise4fun.com/Alive
	+ blog post: http://blog.regehr.org/archives/1170
	+ slides: http://llvm.org/devmtg/2014-10/Slides/Menendez-Alive.pdf
	+ Alive-FP: Automated Verification of Floating Point Based Peephole Optimizations in LLVM - https://www.cs.rutgers.edu/research/technical_reports/report.php?series_id=1&report_id=723
	+ Alive-Loops: https://github.com/rutgers-apl/alive-loops
		- "Termination checking for LLVM peephole optimizations" (ICSE 2016); David Menendez, Santosh Nagarakatte
		- https://www.cs.rutgers.edu/~sn349/papers/icse2016-alive-loops.pdf
	+ Alive-NJ - https://github.com/rutgers-apl/alive-nj
	+ LifeJacket: Verifying precise floating-point optimizations in LLVM - http://export.arxiv.org/abs/1603.09290 - https://github.com/4tXJ7f/alive
	+ Practical Formal Techniques and Tools for Developing LLVM's Peephole Optimizations
		- 2018 PhD Thesis; David Menendez
		- https://www.cs.rutgers.edu/~santosh.nagarakatte/david-menendez-phd-thesis.pdf
	+ Precondition Inference for Peephole Optimizations in LLVM
		- http://export.arxiv.org/abs/1611.05980
		- https://www.cs.rutgers.edu/~santosh.nagarakatte/papers/pldi2017-alive-infer.pdf
		- PLDI 2017 talk, David Menendez - https://pldi17.sigplan.org/event/pldi-2017-papers-precondition-inference-for-peephole-optimizations-in-llvm
	+ Provably Correct Peephole Optimizations with Alive - https://www.cs.utah.edu/~regehr/papers/pldi15.pdf
* CakeML: A Verified Implementation of ML
	+ https://cakeml.org/
	+ https://github.com/CakeML/cakeml
	+ Verified Compilation of CakeML to Multiple Machine-Code Targets. In Certified Programs and Proofs (CPP), 2017.
		- Anthony Fox, Magnus O. Myreen, Yong Kiam Tan, Ramana Kumar.
		- http://www.cl.cam.ac.uk/~mom22/cpp17.pdf
		- http://www.cl.cam.ac.uk/~mom22/publications.html
* CompCert: formally-verified C compiler
	+ http://compcert.inria.fr/
	+ https://github.com/AbsInt/CompCert 
	+ The formal verification of compilers - Xavier Leroy - DeepSpec Summer School 2017
		- https://deepspec.org/event/dsss17/lecture_leroy.html
		- http://gallium.inria.fr/~xleroy/courses/DSSS-2017/
	+ Closing the Gap – The Formally Verified Optimizing Compiler CompCert
		- SSS'17: Safety-critical Systems Symposium 2017
		- https://hal.inria.fr/hal-01399482/
	+ Verified Peephole Optimizations for CompCert
		- PLDI 2016
		- Eric Mullen, Daryl Zuniga, Zachary Tatlock, Dan Grossman
		- http://peek.uwplse.org/
		- https://conf.researchr.org/event/pldi-2016/pldi-2016-papers-verified-peephole-optimizations-for-compcert-
		- Peek: a verified peephole optimizer for CompCert - https://github.com/uwplse/peek
* Compilation Using Correct-by-Construction Program Synthesis
	+ Clément Pit-Claudel; 2016 Master's Thesis at MIT; William A. Martin Memorial Thesis Award for Outstanding Thesis in CS
	+ http://pit-claudel.fr/clement/MSc/
	+ https://dspace.mit.edu/bitstream/handle/1721.1/107293/973557793-MIT.pdf?sequence=1
	+ http://pit-claudel.fr/clement/MSc/FiatToFacade_Pit-Claudel_2016.pdf
* Crellvm: Verified Credible Compilation for LLVM
	+ Programming Languages Design and Implementation (PLDI) 2018
	+ Jeehoon Kang, Yoonseung Kim, Youngju Song, Juneyoung Lee, Sanghoon Park, Mark Dongyeon Shin, Yonghyun Kim, Sungkeun Cho, Joonwon Choi,Chung-Kil Hur, Kwangkeun Yi
	+ a verified credible compilation (or equivalently, verified translation validation) framework for LLVM
	+ http://sf.snu.ac.kr/crellvm/
	+ http://sf.snu.ac.kr/gil.hur/publications/crellvm.pdf
	+ http://sf.snu.ac.kr/gil.hur/publications/crellvm.zip
	+ https://github.com/snu-sf/crellvm-tests-parallel
* Pilsner: A Compositionally Verified Compiler for a Higher-Order Imperative Language
	+ International Conference on Functional Programming (ICFP) 2015
	+ Georg Neis, Chung-Kil Hur, Jan-Oliver Kaiser, Craig McLaughlin, Derek Dreyer, Viktor Vafeiadis
	+ https://people.mpi-sws.org/~dreyer/papers/pilsner/paper.pdf
	+ http://plv.mpi-sws.org/pils/
* Self-compilation and self-verification - Ramana Kumar
	+ http://www.sigplan.org/Awards/Dissertation/2017_kumar.pdf
	+ https://cakeml.org/
* Vale (Verified Assembly Language for Everest)
	+ https://github.com/project-everest/vale
	+ https://www.microsoft.com/en-us/research/publication/vale-verifying-high-performance-cryptographic-assembly-code/
	+ https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/bond
* Vellvm: Verifying the LLVM
	+ http://www.cis.upenn.edu/~stevez/vellvm/
	+ https://github.com/vellvm
	+ Steve Zdancewic - DeepSpec Summer School 2017 - https://deepspec.org/event/dsss17/lecture_zdancewic.html
