# Leaveraging Satellite LiDAR Data for 3D Reconstruction

A python project to use satellite LiDAR data and satellite imagery to create a 3D reconstruction of an area of interest (AOI)

### Environment Setup
For the environment setup using conda makes it easier to setup everything.
The project uses Python version 3.7. Create a conda environment and install following libraries. 
- h5py 
- shapely 
- geopandas 
- pandas 
- geoviews
- holoviews

You can use the following command to create a new conda environment and install the required libraries. 

`conda create -n geditutorial -c conda-forge --yes python=3.7 h5py shapely geopandas pandas geoviews holoviews`

Activate the environment.

`conda activate geditutorial`

If you do not have Jupyter Notebook installed, you may need to run:

`conda install jupyter notebook`


