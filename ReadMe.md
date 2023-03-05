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

`conda create -n GEDI -c conda-forge --yes python=3.7 h5py shapely geopandas pandas geoviews holoviews`

Activate the environment.

`conda activate GEDI`

If you do not have Jupyter Notebook installed, you may need to run:

`conda install jupyter notebook`


### GEDI Finder
- stuff
- stuff
- stuff

### GEDI Level 1B Data 
The GEDI level 1B data contains the processed waveform data. These waveforms can be used get the elevation information. A jupyter notebook to process level 1B data is in the directory 'GEDI_Level_1B_Data'  
The file 'RIT.geojson' stores the geographical boundries of the campus of Rochester Institute of Technology, Rochester New York campus. We will use this file as our area of interest.


