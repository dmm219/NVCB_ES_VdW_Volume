## polarizability:
Contains csv files of the in-plane (xx/yy) and out-of-plane (zz) components of the polarizability tensor in atomic units calculated via QM methods and PISCES.
The number of carbon atoms in the PAH are included as the first column "N_c".
For HF and PBE0, the polarizability components up to N_c=150 are calculated from a 5-pt (F=+/-0.001,0.002) stencil central finite difference of the induced dipole.
For N_c=216 and 294 a 3-pt (F=+/-0.002) stencil central finite difference of the induced dipole was used. 
For MP2 and CAM-B3LYP, the components up to N_c=96 are available and were calculated using the same 5-pt formula.
Confidence is only placed in the first or second decimal place. 

## polarization_potential: 
Contains csv files of in-plane (x) and out-of-plane (z) scans of the polarization potential in atomic units.
The csv files contain the HF, PBE0, model charge+dipole (q+µ), and model dipole (µ) results. 
The distance R is the same in all csv's, but are measured with respect to different origins. 
See the paper for more details. 

## electron_affinities:
Contains csv files of the EOM-EA-CCSD, EOM-EA-MP2, and model EBEs in meV for the charge scaled calculations on coronene. 
The excess molecular charge present while performing the calculation CFOUR is the first column (in atomic units).

## potential_slices:
Contains csv files of the 1D potential slices (in x and y at a fixed vertical separation z) for the interaction of an excess electron interacting with a PAH via the one-electron model in PISCES.
Within the top directory there are folders for each PAH (c6h6, c24h12, etc...).
In each PAH folder, there are folders for each combination of potential terms reported in the paper (polarization, polarization+repulsion, ...).
Within the potential term folders are subdirectories for each value of z the slice was taken taken at.
These folders contain the potential slices as csv files titled as POTENTIAL_*, where * can be X or Y.

