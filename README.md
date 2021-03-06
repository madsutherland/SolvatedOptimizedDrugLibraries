# SolvatedOptimizedDrugLibraries
Here, I take in silico drug screening libraries and run conformer driving in MMFF, then feed the conformers into geometry optimization runs in MOPAC using the PM7 Hamiltonian and the COSMO solvent model. I intend to include the optimized geometries, the annotated code I used to automate these processes, and documentation.

Folder/file convention:
DB_xxx.sdf = the libraries I started with;
initial_geos = molecular structure files for conformers generated in MMFF using OpenBabel's GetConformers functionality;
MOPAC_infiles = input files to energy-optimize atomic coordinates, starting with those in initial_geos, in MOPAC using PM7 and the COSMO solvent model;
MOPAC_outfiles = .out, .arc and .cos files from those MOPAC runs;
optimized_geos = *final, optimized* molecular structures for the conformers, extracted from the MOPAC outfiles, in .xyz format and after conversion to .sdf using Mathematica or Open Babel.



