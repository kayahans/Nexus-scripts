# Nexus-scripts
Depository of scripts used for automated Quantum Monte Carlo calculations

Scripts depend on using Nexus software suite, which is distributed within QMCPACK code (http://qmcpack.org). 

ht_qmc_recipe.py must be copy pasted to /[qmcpack_home]/nexus/library directory

example.py is calculation of an example system (graphene) that can be invoked in any directory. 

Intention is to adapt these scripts as published in J. Chem. Theory Comput., 2017, 13 (5), pp 1943-1951.

- The publication is published using CASINO (https://vallico.net/casinoqmc/) where especially some of the VMC parametrization is already automatized (vmc timestep optimization and on the fly reblocking). QMCPACK doesn't have that capability yet, therefore these would need to be performed with a separate script before using the example.py:
    - vmc_steps: # of steps within a block
    - vmc_dt   : vmc time step

- In these scripts, only diagonally optimal supercells are used, where max lattice vector is minimized. However, a more general form of the supercell matrix should also be implemented. 

- Phonon calculations are missing for now. 






