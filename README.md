Sequential_Sperm_Competition
============================

Code for the study "Female sperm use and storage between fertilization events drive sperm competition and male ejaculate allocation", run in Mathematica 9.0.1.0, platform Mac OS X x86(32-bit, 64-bit Kernel)

In this study, we extend previous sperm competition games in order to incorporate sperm use and storage across consecutive reproductive events based on the volume of ejaculates used during each fertilization event, a simple parameter under female control that influences male success in multiple clutches. In our model, sperm use is the main determinant of sperm competition, which alters the effect of female promiscuity on male success and, ultimately, male reproductive allocation. We adopt the same modeling framework as other sperm competition models (Parker 1998; Parker and Pizzari 2010), but we extend them in two major ways. First, the sperm of a given male does not necessarily compete against all of the sperm previously transferred to his mate, but instead against the amount remaining inside the female's storage organs after she has used some sperm in previous fertilization events. Second, an ejaculate is not only used in the fertilization immediately following mating, but any remaining sperm may also fertilize additional eggs in subsequent clutches.

We performed a numerical search for the evolutionary stable allocation strategy (ESS) in Mathematica 9, where we explored a range of values for the population-level energetic cost per mating, C, between 0.5% and 5% of the total energy budget R each male has available for reproduction. After specifying a value of C, we created a set of all possible allocation strategies that a mutant male may adopt, where the number of mating events obtainged n(s) can only assume integer values. Due to the trade-off between male allocation to pre- and post-copulatory competition, each possible strategy in fact determines corresponding values for n(s) and s. We found the ESSs using an iterated best-response approach (Houston and McNamara 1987), which consisted of: (1) setting a specific strategy as the initial one adopted by the wild-type males in the population, (2) evaluating the performance of mutant males adopting the alternative strategies, (3) setting the strategy that achieved the highest fitness as the strategy adopted by the wild-type males in the population in the next iteration, (4) repeating the evaluation of alternative strategies until reaching the Nash equilibrium, where the best response for a given wild-type strategy is adopting exactly the same strategy. Given that we used every strategy as the initial condition in alternative runs during the numerical search for the best response strategy, we were also able to check for the convergence of the same best response under different initial conditions, which we considered the ESS. For a small number of parameter combinations, the best response procedure cycled between two neighboring solutions. Finally, we also evaluated the ESS allocation over different levels of sperm use (parameter u, ranging from 0.01 to 1.00).

References:

Houston, A. I., and J. M. McNamara. 1987. Singing to attract a mate: a stochastic dynamic game. J. Theor. Biol. 129:57-68.

Parker, G. A. 1998. Sperm competition and the evolution of ejaculates: towards a theory base. Pp. 3–54 in T. R. Birkhead, and A. P. Møller, eds. Sperm competition and sexual selection. Academic Press, New York.

Parker, G. A., and T. Pizzari. 2010. Sperm competition and ejaculate economics. Biol. Rev. 85:897–934.


Acknowledgments:

Special thanks to Daniel S. Caetano (https://github.com/Caetanods) for helping creating and uploading the files into this repository
