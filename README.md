Molecular dynamics

A molecular dynamics simulation code has been created for relativistic and electromagnetic fields in three dimensions, and is used such as nanoscale particle phenomena. Maxwell equations are solved, and the momentum equations of relativistic particles are then advanced in time. But, it is noted that the Gauss's equation must be corrected as finite errors accumulate in the divergence term. This is true if a discrete coordinate scheme in any method is utilized.

All explicit simulation code must satisfy the Courant condition, that is, Dx(length)/Dt(time step) > c, the speed of light. 
Four physical CGS units are used in this code: a_unit= 1.00d-08 cm, t_unit= 1.00d-15 sec, electron mass m_unit= 0.9110d-27 g and its charge e_unit= 4.8032d-10 esu. The mass of hydrogen, for example, is 1.6726d-24 g. One needs files in the simulation: 1) @cnt3-3p8Ca.f03: Molecular dynamics simulation code, 2) param_em3p8_Ca.h: Common parameters of this simulation, 3) Cntemp_config.STARTC: figure parameters, 4) p_config_ss.xyz_D150 and P135: 4) Pellet electrons, H, C and Au ions. The program is written in Fortran 2003 and MPI version 3 for parallelization.

A simulation of the nanotube accelerator is set up by putting pellets of H, C and Au atoms and associated electrons at null velocity. 
Electromagnetic monochromatic waves at the wavelength 800 nm are travelling from the negative direction toward the origin and then go out to the positive direction. The pellets at the origin are irradiated by these waves and are ejected to ion perpenducular and electron parallel directions toward an open space. The final energies for laser intensity 10^22 W/cm^2 are around 30-40 MeV in 20-40 fs, which is shown by animation movies at my homepage. 
It is discussed in the latter half of CPC paper (2019).

Finally, the machine run time depends on the physical time and cpu's architecture. 
For the elapsed time of parallel execution was 4.0 sec/step for 52 ranks and 4.0 10^5 particles
(or 1 fs for elapsed circa 3 hours) by Fujitsu FX100 Supercomputer.  


References:

1. M. Tanaka and M. Murakami, Relativistic and electromagnetic molecular dynamics simulations for a carbon-gold nanotube accelerator, Computer Physics Communications, 241, 56-63 (2019).

2. M. Tanaka, A simulation of low-frequency electromagnetic phenomena in kinetic plasmas of three dimensions, J.Comput. Phys., 107, 124-145 (1993).

3. M. Murakami and M. Tanaka, Generation of high-quality mega-electron volt proton beams with intense-laser-driven nanotube accelerator, Applied Phys. Letters, 102, 163101 (2013).

