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

the same setup and dependencies can be achieved by using another package manager such as `pip`


### GEDI Finder
GEDI Orbit granules over a certion region can be found using a GEDI Finder. A bounding box can be defined using Longitude and Lattitude and the script query the base CMR granule search url to get a list of all the orbit granules over Area of interest.  
You can use another script `DAACDataDownload.py` to download all the data files. The execution command to data downloader script is as below  
`python DAACDataDownload.py -dir <insert local directory to save files to> -f <insert a single granule URL, or the location of a csv or text file containing granule URLs>`

### GEDI Level 1B Data 
The GEDI level 1B data contains the processed waveform data. These waveforms can be used get the elevation information. A jupyter notebook to process level 1B data is in the directory 'GEDI_Level_1B_Data'  
The file 'RIT.geojson' stores the geographical boundries of the Rochester Institute of Technology, Rochester New York campus. We will use this file as our area of interest.

:earth_americas: You can use data downloader script from GEDI Finder to get required data. Alternatively you can visit the [NASA Earthdata Search website](https://search.earthdata.nasa.gov/search) to download the required data

