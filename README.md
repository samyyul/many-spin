# Optimisation of eigenvalues using EigOpt #
## Summary ##

EigOpt was birthed from a spectulative master's project, where I was tasked to produce a code to reliably optimise exchange couplings to Eigenvalues for many-spin body systems. 

Exchange (J) couplings are initially determined using Broken Symmetry Density-Functional Theory (BS-DFT). This method is easy and provides a reasonable initial approximation for J couplings. Diagonalisation of a Heisenberg Hamiltonian matrix produced with these values proves it is indeed an approximation: the elucidated eigenvalues pail in accuracy when compared to those calculated using multi-reference methods, such as Dedicated Difference Configuarational Interaction (DDCI) and Complete active space self-consistent Field (CASSCF). The caviate to these higher-level methods is that they do not output any exchange couplings! So we have two equally important quantities, which are differing substantially in accuracy! How do we solve this crisis of inequality?

Our Solution was EigOpt, a script that optimises our approximated J-couplings to our reliably calculated eigenvalues.

## Github Scripts ##
### ** This code has been superceded ** ### 

Our original work is visable in two seperate python scripts, which are open for use and toying with:
- Optimise_2 : Provides optimised J couplings, which are then used in Heisenberg.
- Heisenberg : Provides a detailed output of eigenvalues, eigenvectors and multiplicity.

The combintation of these two scripts provides the neccessary framework to accurately elucidate exchange coulings for your target system, and was used to verify results for my Master's Thesis.

While successful in it's goal, There were a number of objectives we envisioned early-on that could not fit into the timescale of a 8-month Master's project. Fortunately, Our department a the University of Manchester saw the potential of our work, and granted extra research time so that we could develop our project to match our vision. 

## EigOpt Website ##

The additional research time enabled us to transform our python scripts into a flask-based web appilcation. This satified are primary goal of making our utility accessible for non-specialist researchers, who may be less familar with computational/theoretical concepts.

Other key developments include:

- changing from a home-cooked Heiesenberg Code to a Quspin-based code,  making the code less restrctive for future developments.
- 
- Addition of an interactive tool to visualise exchange couplings.
  
- Addtional flexbility when choosing variable(s) to optimise.


