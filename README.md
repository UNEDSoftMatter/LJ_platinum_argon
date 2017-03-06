#LJ_platinum_argon

lammps MD scripts to perform the simulation of fluid argon between two platinum walls when the temperature of the walls is increased. Because of the pbc and absence of vacuum between the border of the walls and the border of the simulation box, we can considerar the two walls as only one. So, the simulation perform a solid platinum walls surrounded by a fluid argon.


__in.walls__ performs the complete simulation (equilibration and production stages).__in.walls.equilibration__ only equilibration stage and __in.walls.production__ production stage.  

The input lammps files __in.walls.vacuum__, __in.walls.equilibration.vacuum__ and __in.walls.production.vacuum__ performs the same system with vacuum between the bottom of the simulation box and the first layer of the lower solid, and between the last layer of the upper solid and the top of the simulation box.  I use the first option (without vacuum).

The simulation has three parts: 
- In microcanonival ensemble, fluid and walls reach equilibrium with a langevin thermostat (T= 1.5)
- Once the system is equilibrated, the temperature of the wall is increased (T = 10). 
- Then, the system reaches the equilibrium. 

The process is performed in the microcanonical ensemble. 

A Lennard-Jones potential is used with parameters from _Molecular dynamics study of effect of different wetting conditions on evaporation and rapid boiling of ultra-thin argon layer over platinum surface_. S.M. Shavik, Mohammad Nasim Hasan, A.K.M. Monjur Morshed, M. Quamrul Islam.
 
