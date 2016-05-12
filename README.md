#LJ_platinum_argon

lammps MD scripts to perform the simulation of fluid argon between two platinum walls when the temperature of the lower wall is increased.

The script has three parts: 
1. In microcanonival ensemble, fluid and walls reach equilibrium with a langevin thermostat (T= 1.5)
2. Once the system is equilibrated, the temperature of the lower wall is increased (T = 10). 
3. Then, the system reaches again the equilibrium. 

The process is performed in the microcanonical ensemble. 

A Lennard-Jones potential is used with parameters from _Molecular dynamics study of effect of different wetting conditions on evaporation and rapid boiling of ultra-thin argon layer over platinum surface_. S.M. Shavik, Mohammad Nasim Hasan, A.K.M. Monjur Morshed, M. Quamrul Islam.
 