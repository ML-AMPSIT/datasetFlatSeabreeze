# Dataset of flat terrain ideal simulations of seabreeze

This dataset was used for a sensitivity analysis performed with ML-AMPSIT, available at http://dx.doi.org/10.5281/zenodo.10789930. The analysis was performed using WRF4.4 (doi:10.5065/D6MK6B4K) simulations perturbing 6 parameters of the land surface model Noah-MP, as described in the paper "ML-AMPSIT: Machine Learning-based Automated Multi-method Parameter Sensitivity and Importance analysis Tool" (10.5194/gmd-2024-56).

## Descritpion

The present dataset contains the input perturbation file X.txt, the configuration file configAMPSITseabreeze.json, and 3 folders, each containing simulation data from a pair of domain points, over the land surface and water surface of the simulation domain, respectively.
The analyses performed on these data use an average of three adjacent cells in the south-north direction. The central points of these two locations are x=100, y=95 and x=100, y=105 for water and land respectively, i.e. in the central cell in the west-east direction, and 5 grid points to the north and south of the land-water interface.
The data for the central pair are contained in the centralPoint folder, and the other two adjacent pairs are contained in the upperPoint and lowerPoint folders. 
Each folder contains data files named V_MEAN_land_wrfout_d01_2015-03-20_18_00_00_* and V_MEAN_water_wrfout_d01_2015-03-20_18_00_00_* for land and water, respectively, where * refers to the simulation member of the ensemble.
Each file contains an NxM matrix, where N is the number of vertical levels and M is the number of simulated time steps.
The preprocessing of these data as well as the subsequent analyses were performed with the tools provided in ML-AMPSIT, available at http://dx.doi.org/10.5281/zenodo.10789930.
