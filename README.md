# Dataset of flat terrain ideal simulations of seabreeze

## Descritpion

The present dataset contains the input perturbation file X.txt, the configuration file configAMPSITseabreeze.json, and 3 folders, each containing simulation data from a pair of domain points, over land surface and water surface of the simulation domain respectively.
The analyses performed over these data uses an average output from three adjacent cells in the south-north direction. The central points of these two locations are x=100, y=95 and x=100, y=105 for water and land respectively, i.e. in the central cell in the west-east direction, and 5 grid points to the north and to the south of the land-water interface.
The central pair data are contained in the centralPoint folder. the other two adjacent pairs are contained in upperPoint and lowerPoint. 
Each folder contains data files entitled V_MEAN_land_wrfout_d01_2015-03-20_18_00_00_* and V_MEAN_water_wrfout_d01_2015-03-20_18_00_00_* for land and water respectively, where * refers to the simulation member of the ensemble.
Each file contain a NxM matrix where N is the number of vertical levels and M is the number of simulated time steps.
the pre-processing of these data, as well as the subsequent analyses have been performed with the tools provided in ML-AMPSIT available at http://dx.doi.org/10.5281/zenodo.10789930 .
 
