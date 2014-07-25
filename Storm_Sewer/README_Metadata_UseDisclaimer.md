# City of San Jose Storm Sewer Features

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
This data details the City of San Jose's storm sewer features.  It is updated monthly from the City's GIS database.

## Metadata
###Attribute Fields
####Storm_Inlet
`STM_INL_ID` Storm Inlet ID  
`PCD_TYPE` Type of pollution control device  
`PCD_IN_DAT` Date pollution control device was installed  
`PCD_MANUF` Manufacturer of pollution control device  
`STATUS` Status of particular asset indicating usage  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`QTR_PL_OLD` Store legacy quarter panels information from old City grid(prior to adjustment to County Grid)  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`RIM_ELEV` Elevation (feet) of rim of inlet in NGVD29 or datum unknown  
`DEM_RM_N88` Elevation (feet) of rim of inlet in NAVD88 based on GIS location relative to LiDAR DEM  
`OUTLET_INV` Invert elevation (feet) of inlet where it drains into lateral(datum unspecified or unknown)  
`LONG_NAD83` Longitude of point location, populated through a spatial trigger  
`LAT_NAD83` Latitude of point location, populated through a spatial trigger  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`ADDL_INLET` Flag that indicates a "new" inlet put in by MRF during rubbersheeting  
`IN_W_O_LAT` Inlet without Lateral, locations of missing inlets identified by DOT maintenance staff  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Lateral
`STM_LA_ID` Lateral ID  
`STATUS` Status of particular asset indicating usage  
`MATERIAL` Material of lateral  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`UPSTR_INV` Invert (feet) elevation of inlet flowing into lateral(NGVD 29 or datum unknown)  
`UP_INV_N88` Invert value at upstream inlet NAVD88(if datum known)  
`DN_STR_INV` Invert elevation(feet) value downstream of inlet where lateral flows into pipe, manhole, or basin(NGVD 29 or datum unknown)  
`DN_INV_N88` Invert elevation(feet) value at downstream inlet NAVD88(if datum known)  
`DIAMETER` Diameter of the lateral in inches  
`LENGTH` Length of the lateral in feet from plan  
`LENGTH_MEA` Measured length of the lateral in feet from GIS  
`SLOPE` Plan slope (unitless) of pipe segment, always auto-calculated from upstream and downstream invert  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`LA_W_O_INL` Lateral without inlet  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Main
`STM_MN_ID` Auto incremented artificial primary key  
`DISTATT_ID` Auto incremented artificial primary key unique for this table  
`OUTFALL_ID` Outlet Outfall ID for the network that storm main system is part of  
`OUTFALL_GP` Outlet Outfall Group ID for the network that storm main system is part of  
`UP_STR_TYP` Type of asset upstream asset ID refers to(manhole, basin, pump station, or cap)  
`UP_STR_ID` ID of the upstream asset(manhole, basin, pump station, or cap)  
`UP_STR_INV` Elevation in feet of end of pipe at upstream manhole(assumed to be NGVD29, or unknown)  
`DN_STR_TYP` Type of asset downstream asset ID refers to(manhole, basin, pumpstation, or cap)  
`DN_STR_ID` ID of the downstream asset(manhole, basin, pumpstation, or cap)  
`DN_STR_INV` Invert elevation (feet) at downstream assumed to be in NGVD29, or datum unknown  
`DOWNSTR_INVERT_NAVD88` Invert value at downstream manhole in NAVD88(if datum known)  
`TYPE` Type of main  
`SYPHON_TYP` SYPHON type of storm main  
`STATUS` Status of particular asset indicating usage  
`MATERIAL` Material of storm main  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`START_MEAS` Start measurement of main used for dynamic segmentation of mains  
`END_MEAS` Calculated end measurement of the main  
`LENGTH` Length of the lateral in feet from plan  
`LENGTH_MEA` Measured length of the lateral in feet from GIS  
`SLOPE` Plan slope (unitless) of pipe segment, always auto-calculated from upstream and downstream invert  
`DIAMETER` Diameter of the lateral in inches  
`CAPACITY` Main capacity in MGD for full pipe  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`NO_OUTFALL` Last downstream storm main that ends without an outfall ID  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`PIPE_SHAPE` Shape of the main  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Manhole
`STM_MH_ID` Manhole ID  
`COMPKEY` Matching Hansen ID for asset in SSMS Hansen Asset Management System  
`COMPTYPE` Matching Hansen asset type identifier in SSMS Hansen Asset Management System  
`TYPE` Manhole type  
`PCD_TYPE` Type of pollution control device  
`PCD_IN_DAT` Date pollution control device was installed  
`PCD_MANUF` Manufacturer of pollution control device  
`STATUS` Status of particular asset indicating usage  
`MATERIAL` Manhole material  
`LOCKING` Is manhole locked, yes or no  
`BYPASS` If manhole has two outgoing pipes such that the upper will bypass the lower once a certain flood level is reached  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`RIM_ELEV` Elevation (feet) of rim of inlet in NGVD29 or datum unknown  
`DEM_RM_N88` Elevation (feet) of rim of inlet in NAVD88 based on GIS location relative to LiDAR DEM  
`LOW_INV_EL` Lowest invert elevation in feet  
`MH_BTM_EL` Elevation (feet) at bottom of manhole(NGVD29 or unknown datum Derived by subtracting from 4 to 8 inches from the lowest invert elevation depending on the diameter of the lowest outgoing main)  
`MH_BTM_N88` Elevation (feet) at bottom of manhole (NAVD88)(if datum known)  
`COVER_DIAM` Diameter of manhole cover in inches  
`DETAL_LINK` Link to documents, plans, and photos(to be populated in the future)  
`QUALTY_LEV` Spatial accuracy of manhole location  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`REHAB_DATE` Date manhole was rehabilitated  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Outfall
`STM_OTF_ID` Outfall ID  
`COMPKEY` Matching Hansen ID for asset in SSMS Hansen Asset Management System  
`COMPTYPE` Matching Hansen asset type identifier in SSMS Hansen Asset Management System  
`TYPE` Type of outfall  
`PCD_TYPE` Type of pollution control device  
`PCD_IN_DAT` Date pollution control device was installed  
`PCD_MANUF` Manufacturer of pollution control device  
`STATUS` Status of particular asset indicating usage  
`FLAP_BRAND` The brand of flapgate the outfall has, if the outfall has a flapgate  
`AGENCY` Date that any attribute was changed  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`LONG_NAD83` Longitude of point location, populated through a spatial trigger  
`LAT_NAD83` Latitude of point location, populated through a spatial trigger  
`DETAL_LINK` Link to plan, photo or other document or file(to be populated in the future)  
`QUALTY_LEV` Spatial accuracy of manhole location  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Overland_Drain
`STM_O_D_ID` Overland Drain ID  
`TYPE` Type of overland drain  
`PCD_TYPE` Type of pollution control device  
`PCD_IN_DAT` Date pollution control device was installed  
`PCD_MANUF` Manufacturer of pollution control device  
`STATUS` Status of particular asset indicating usage
`MATERIAL` Material of overland drain  
`PURPOSE` Purpose of overland drain  
`USE` Use of overland drain  
`LOCATION` Where the OVERLAND DRAIN was placed, whether it was within right-of-way or easement  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WIDTH` Width of overland drain in inches  
`LENGTH` Length of the lateral in feet from plan  
`DEPTH` Depth of overland drain in inches  
`OUTLET_INV` Invert elevation in feet at end of overland drain where water dumps out  
`SHAPE` Shape of overland drain  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  

####Storm_Pumpstation
`ST_PUMP_ID` Pump station ID  
`COMPKEY` Matching Hansen ID for asset in SSMS Hansen Asset Management System  
`COMPTYPE` Matching Hansen asset type identifier in SSMS Hansen Asset Management System  
`LOCATION` Location of pump station  
`UNDERPASS` Pumpstation is under or associated with an underpass  
`OWNER` Maintenance jurisdiction of asset (e.g. San Jose, Burbank, Sunol, Santa Clara, Milpitas, Campbell, Saratoga)  
`QTR_PANEL` Quarter panel which the longest portion of the main resides  
`WATERWAY` The waterway that the contents of the main spill to  
`MAJ_W_SHED` The major watershed in which the largest portion of the main resides  
`NU_OF_PUMP` Number of pumps for pumpstation(from DOT spreadsheet)  
`N_CAP_GPM` Nominal capacity of pumpstation in gallons per minute(from DOT spreadsheet)  
`NOMINAL_HP` Nominal horsepower of pumps(from DOT spreadsheet)  
`DETAL_LINK` Link to plan, photo or other document or file(to be populated in the future)  
`QUALTY_LEV` Spatial accuracy of manhole location  
`REC_DRAW` Plan used to enter asset is or is not a record drawing(Boolean)  
`OTH_PN_CRE` Plan that created asset  
`OTH_PN_MOD` Plan that modified asset  
`CONST_DATE` Date construction plan was signed or date minus six months that record drawing was signed  
`ACCEP_DATE` Date record drawing was signed or date plus six months that construction plan was signed  
`YEAR_UPGRD` The year the pump station was upgraded(from DOT spreadsheet)  
`AT_MOD_DAT` Date that any attribute was changed  
`GE_MOD_DAT` Date geometry first entered or last modified  
`MESSAGE` Message from automated batch process to operator; can be "OK", or error message, or "to be checked ", or any free form message about the asset  


### Projections
* GeoJSON, and KMZ files are in WGS84 coordinate system.
* The zipped files are shapefiles in NAD_1983_StatePlane_California_III_FIPS_0403_Feet projected coordinate system.

###Source
City of San Jose - Public Works GIS Team  
200 East Santa Clara Street  
San Jose, CA 95113  
