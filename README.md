# VIIRS

There are five files associated with VIIRS.

### 1) Dump 
a) Read the fileList and the get read the Dataset file that is listed. <br />
b) Get the date and time variable and map it along the size of the data array. <br />
c)Loop through all the sds variables and find "Aerosol_Optical_Thickness_550_Land", "Aerosol_Optical_Thickness_550_Land_Ocean_Best_Estimate", "Aerosol_Optical_Thickness_QA_Flag_Land", "Aerosol_Type_Land_Ocean" and "Angstrom_Exponent_Land_Ocean_Best_Estimate". <br />
d) Add columns for each one and list the values. <br />
e) Create excel sheet list all the data for these variables along with the date and time when they were collected. <br />

### 2) List
a) Read the fileList and the get read the Dataset file that is listed. <br />
b) The main function call another function to print the following values:<br />
  i) nc_attrs : list<br />
       &emsp; A Python list of the NetCDF file global attributes<br />
   ii) nc_dims : list<br />
       &emsp; A Python list of the NetCDF file dimensions<br />
   iii) nc_vars : list<br />
        &emsp;A Python list of the NetCDF file variables<br />


### 3) At a Location
a) Read the fileList and the get read the Dataset file that is listed. <br />
b) Calculate the mean, median and standard deviation and display them. <br />
c) Calculate the range of valid data and display the longitude and lattitude. <br />
d) User should input longitude and latitude that fall within the range.<br />
e) Calculate points that are closest to the user input and identify if those point fall under a three by three or a five by five grid.<br />

### 4) Map
a) Read the fileList and the get read the Dataset file that is listed. <br />
b) Promt the user to choose between  "Aerosol_Optical_Thickness_550_Land", "Aerosol_Optical_Thickness_550_Land_Ocean_Best_Estimate", "Aerosol_Optical_Thickness_QA_Flag_Land", "Aerosol_Type_Land_Ocean" and "Angstrom_Exponent_Land_Ocean_Best_Estimate". <br />
c) Calculate the range of valid data to be used to be displayed in the map. <br />
d) Plot the heat map along with a color bar on the side based on the sds variable chosen and the data for that variable.<br />

### 5) Calculate PM2.5
a) Read the fileList and the get read the Dataset file that is listed. <br />
b) Promt the user to choose between  "Aerosol_Optical_Thickness_550_Land", "Aerosol_Optical_Thickness_550_Land_Ocean_Best_Estimate", "Aerosol_Optical_Thickness_QA_Flag_Land", "Aerosol_Type_Land_Ocean" and "Angstrom_Exponent_Land_Ocean_Best_Estimate". <br />
c) Calculate the range of valid data to be used to be displayed in the map. <br />
d) Based on the data seperate the quality of the aerosol. <br />
e) Plot the heat map along with a color bar on the side based on the sds variable chosen.<br />
