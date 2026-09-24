# SEOF
Code for SEOF calculations in line with Maher et al, 2026 Climate Dynamics


For the scripts outlined below there are often versions for different variables, for the ensemble and the time dimension, and for models where the historical + future scenario are in a single file or when they are in two files. Outlined below are the classes of scripts used in the analysis. 

The Figures scripts are labelled by their Figure number. 

Analysis scripts:

execute_SEOF_ 
Script: this piece of code runs the SEOF package on single file input for 500mb geopotential height in the PNA and NAt regions

Output files: SEOFs for North Pacific & North Atlantic

PNA & NAT

SEOF, SPCS, FVAR, TVAR

For each model the z500 fields with and without the ensemble mean removed. 
_zgDJFerem
_zgDJF'

process_precip_
Script: this piece of code loads and processes precipitation files for single inputs for use later in plotting scripts

Notes: needs to be run individually for each model - check the boxes that have a *change me* tag on the top. 

For each model the pr field with the ensemble mean removed. 
DJFerem


load_regress_plot 
Script: loads the SEOF, regresses on 500mb geopotential height, then plots panels - similar to O'Brien & Deser Figure S1, Figure 1


For Npac Tpac and NAT
Output files for plotting:
FS1bdata_zg
F1bdata_zg
SPCs_zg


Figure6_
Script: regresses out the Tropical Pacific influence and plots preci similar to O'Brien & Deser Figure 6

Output files for plotting:
F6data_pr
F6data_zg
