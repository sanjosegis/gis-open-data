# City of San Jose Sanitary Sewer Features

## Use Disclaimer
Please be advised that the City does not warrant the accuracy of the GIS (Geographic 
Information Systems) data.  This data is provided to you "as is," and you agree to use it 
at your own risk.  The City makes no guarantees, representations or warranties of any kind, 
express or implied, arising by law or otherwise, including but not limited to,
content, quality, accuracy, completeness, effectiveness, reliability, fitness for a 
particular purpose, usefulness, use or results to be obtained from this data, or that the 
data will be uninterrupted or error-free.  By downloading and/or using this data, you agree 
that any use of, and reliance upon, the data wil be at your sole discretion and risk, and you 
agree to take full responsibility therefore.

##Overview
This data details the City of San Jose's sanitary sewer features.  It is updated monthly from the City's GIS database.

## Metadata
###Attribute Fields
####Sanitary_Main
`MAIN_ID` Sanitary main ID  
`DISTATT_ID` Auto incremented artificial primary key unique for this table  
`PLAN_CREAT` This is the number of the plan that created the pipe and can be an improvement, discrepancy or othe plan type  
`PLAN_MOD` This is the number of the plan that modified the pipe after creation and can be an improvement, discrepancy or othe plan type  
`SD_DAT_ELV` Calculated datum elevation in feet  
`PL_DAT_ELV` Plan datum elevation in feet  
`STATUS` Status of particular asset indicating usage  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`SRC_YR_BLT` Source year built  
`YEAR_BUILT` Year built  
`UP_STR_INV` Elevation in feet of end of pipe at upstream manhole (assumed to be NGVD29, or unknown)  
`UP_S_MH_ID` Upstream manhole ID  
`UP_S_MH_NA` Upstream manhole name  
`DN_S_MH_ID` Downstream manhole ID  
`DN_S_MH_NA` Downstream manhole name  
`DN_STR_INV` Invert elevation (feet) at downstream manhole assumed to be in NGVD29, or datum unknown  
`LENGTH` This is the actual length of the pipe (in feet) derived from the improvement plan  
`LNTH_MEAS` This is the measurement of the pipe geometry (in feet) derived by the GIS system  
`TYPE` Type of main  
`SLOPE` Plan slope (unitless) of pipe segment, always auto-calculated from upstream and downstream invert  
`MATERIAL` Sewer pipe material from lookup table(ie VCP = vitrefied clay pipe, CIP = cast in place, LIN = in situ to form)  
`DIAMETER` Diameter of the pipe in inches  
`CAPACITY` Sewer capacity  
`START_MEAS` Uses for linear referencing  
`AT_MOD_DAT` Attribute modified date  
`END_MEAS` Uses for linear referencing  
`GE_MOD_DAT` Geometry modified date  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Sanitary_Manhole
`MANHOLE_ID` This is the unique primary key for the SAN_MANHOLE table  
`TYPE` This is the type of manhole  
`MATERIAL` This is the material of the manhole  
`STATUS`  Status of particular asset indicating usage  
`RIM_ELV` This the elevation at ground level of the manhole rim  
`LO_INV_ELV` This is the elevation of the lowest invert connected to the manhole  
`GE_MOD_DAT` Geometry modified date  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  
`DEM_RIM_EL` Rim elevation measured from DEM  
`AT_MOD_DAT` Attribute modified date  

### Projections
* GeoJSON, and KMZ files are in WGS84 coordinate system.
* The zipped files are shapefiles in NAD_1983_StatePlane_California_III_FIPS_0403_Feet projected coordinate system.

###Source
City of San Jose - Public Works GIS Team  
200 East Santa Clara Street  
San Jose, CA 95113  
