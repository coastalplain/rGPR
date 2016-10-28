# rGPR
Tools to work with various ground-penetrating radar (GPR) data files.  FIRST, navigation to shapefile.

rGPR is just starting.  It should be a system used to recursively find any type of GPR files on your system, 
create ArcGIS shapefiles or file geodatabases, and create point and line files from navigation in the field.  
Eventually, we should be able to convert the native format GPR files into standard SGY files for storage, but 
into rGPR format for processing and viewing in R.

In coastalplain/MALA-GPR I have created a crude way to recursively extract MALA gpr coordinate files from a large
number of hard drives and create a shapefile so I know where what data set is located.

What I would like to be able to do efficiently, but am slowly learning (feel free to suggest and jump in!), is to
work with all formats of GPR data, convert them and their navigation to a cross-platform capability (in R, 
use "rgpr" format; for permanent storage and reloading using rGPR, SEG-Y format).

I would like to create a package that any of my (our) colleagues can use that will allow:
  1.  File finding, file name manipulation, bulk rename and move, etc.
  2.  Creation of R-compatable files, and files for ArcGIS or eventually Q-GIS/OpenGIS
      a. Working with available navigation, or creating navigation for a GPR file or GPR grid by placing on a map :)
      b. Create a R-useable format for plotting navigation on a nice map
      c. Create a Geodatabase from scratch, adding the navigation, and adding the SEG-Y data as blobs or files in the Geodatabase
      d. Be able to extract original data or processed data from the geodatabase
  3.  Conversion from native format to .rgpr format and to SEG-Y format
  4.  Data processing in 2D (filtering, processing, etc. including time-domain and frequency-domain)
  5.  2D visualization and plotting
  6.  3D processing with grids of 2D or true 3D data (much later, I'm guessing...)
  
  NOTES:  
     maybe come up with an .rgeo file, that could be GPR, seismics, geochronology, or other geo-based dataset?
     
