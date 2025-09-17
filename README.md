# EigOpt: Optimisation of Eigenvalues  

A Python-based framework to optimise exchange couplings (J) in Heisenberg Hamiltonians against target eigenvalues, developed from my Master's research.
## Summary 

EigOpt originated from my master's project, where I developed a code to optimise exchange couplings (J)  for many-spin systems. 

**Motivation**

- Exchange (J) couplings are initially determined using Broken Symmetry Density-Functional Theory (BS-DFT). 
- This method is easy and provides a reasonable initial approximation for J couplings. 
- The calculated eigenvalues with BS-DFT pale in accuracy when compared to those calculated using multi-reference methods, such as Dedicated Difference Configuarational Interaction (DDCI) and Complete active space self-consistent Field (CASSCF). 
- The caviate to these higher-level methods is that they do not output any exchange couplings.

Our Solution was EigOpt, a script that optimises our approximated J-couplings to our reliably calculated eigenvalues.

## Original Python Scripts (archived)  

The initial version of EigOpt is available in two standalone scripts:  

- **Optimise_2.py** – optimises J couplings to match target eigenvalues.  
- **Heisenberg.py** – calculates eigenvalues, eigenvectors, and multiplicities.  

These scripts form the core framework used in my Master's thesis. While functional, they have since been superseded by the web application (see below).  

While successful in it's goal, There were a number of objectives we envisioned early-on that could not fit into the timescale of a 8-month Master's project. 

## Web application 

Following the initial success, EigOpt was extended into a **Flask-based web application** to improve accessibility for researchers without a computational background.  

**Key features:**

- Migration from custom Heiesenberg Code to  **Quspin**,  enabling broader functionality and making future developments less troublesome.

- interactive **visualisation** tool for exchange couplings.
  
- Flexbility choice of variable(s) for optimisation.

- Hosted on a university virtual machine, with ongoing development planned.  




