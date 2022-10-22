Two preparatory steps are required in order to implement this analysis in the same manner.


------------------------------------------------------------------


1 - All libraries and dependencies must be installed.


To begin with, GDAL dependency must be installed since it is the basis for a number of libraries that will be used

In Linux: sudo apt-get install libgdal-dev
in Conda: conda install -c conda-forge gdal

---------

Once that is completed, in the shell or command line run below:

- CD to directory where the requirements.txt is located. (This project folder in this case)
- Activate your virtual enviroment. If you are not working in a virtual environment, skip this step
- run -> In Linux: -> pip install --file requirements.txt
  run -> In Conda: -> conda install --file requirements.txt

--------------------------------------------------------------------------

2 - Download the climate dataset and copy it to the "./climate" directory in the project folder, 
There are two files one for temperature and one for precipitation and the file format is ".NC" , 
there are two ways to get the data:


Download from the source website World Bank Climate Change Knowledge Protal (CCKP) "https://climateknowledgeportal.worldbank.org/download-data"
In the second half of the webpage, there are download options for four main categories (Map, Climatology, Timeseries, heatplot). The requirement for this project is the data under the "Map" category and the parameters as below

Parameters for Temperature as below
Collection: ERA5 (Reanalysis)
Climatology: Timeseries (1950 - 2020)
Variable: Mean_Temperature
Aggregation: Annually

Parameters for Precipitation as below
Collection: ERA5 (Reanalysis)
Climatology: Timeseries (1950 - 2020)
Variable: Precipiation
Aggregation: Annually


Alternatively, I uploaded the same data used at the time of producing the this paper on google drive (Download Link: "https://drive.google.com/drive/folders/1Ie6mDiyvgXODL85ZoChGM_VqQJYwi5fy?usp=sharing"), the data can be downloaded from there.

Once both files are downloaded copy both files to the "./climate" directory in the project folder.