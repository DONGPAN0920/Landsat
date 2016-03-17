# Landsat
Python project that handles Landsat data processing

*Requires __Functions.py__ from the [GDAL_Python3](https://github.com/jdegene/GDAL_Python3) repository*, make sure its in the PYTHONPATH


### LS.py

Uses original *.tar.gz packed Landsat 4,5,7 or 8 files (e.g. from http://earthexplorer.usgs.gov/) in an input folder, 
creates a subfolder with the Landsat name and:
* extracts bands
* calculates radiation bands
* calculates TOA reflection bands
* calculates surface temperature in Kelvin
* calculates one or all indices (NDVI, EVI, SAVI, MSAVI, NDMI, NBR, NBR2, NDSI) according to the [Landsat Surface Reflectance High Level Data Products](http://landsat.usgs.gov/CDR_LSR.php)

The script uses flags to determine if intermediate outputs should be saved as rasters to HDD or removed after the process is finished