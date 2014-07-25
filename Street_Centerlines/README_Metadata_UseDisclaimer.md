# City of San Jose Street Centerlines

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
This data details the City of San Jose's street centerline datasets.  It is updated monthly from the City's GIS database.

## Metadata
###Attribute Fields
####DIVIDED_STREETS
`PID MASTER_ID` ID of the street name from BAS_STREET_MASTER table  
`PREFIX` Street directional prefix  
`NAME` Street name  
`SUFFIX` follows the name of a street to further describe that street  
`TYPE` Street type abbreviation(Road = Rd, Street = St, Avenue = Ave, Court = Ct, etc)  
`CLASS` A 2 char representation of allowable values for street classes: HY(highway), EX(expressway), MA(major arterial), MI(minor arterial), CO(collector), RE(residential, neighborhood), AL(alleyway), EA(easement)  
`ROW_WIDTH` Width of right-of-way(international feet)  
`FOC_WIDTH` Distance from top of the curb on one side of the street to the top of the curb on other side of the street  
`ADD_TYPE` The type of address sequences are standard even side-odd side numbering, contiguous numbering such as in a cul-de-sac, other numbering schemes  
`FRADD_L` Address range limitation for the LEFT street side at the starting point of the digitization  
`FRADD_R` Address range limitation for the RIGHT street side at the starting point of the digitization  
`TOADD_L` Address range limitation for the LEFT street side; at the end point of the digitization  
`TOADD_R` Address range limitation for the RIGHT street side at the end point of the digitization  
`MUNI_L` Name of municipality on the left side of the street segment  
`MUNI_R` Name of municipality on the right side of the street segment  
`ZIP_L` Zip-code on the left side of the street segment  
`ZIP_R` Zip-code on the right side of the street segment  
`PRIVATE` A character flag (Y/N) that indicates if the street is private or public  
`ONE_WAY` Contains values for street segment direction flags:'B' -2 way street. 'P'-one way with traffic to the same direction as segment digitized. 'N'-one way with traffic in opposite direction as segment digitized. 'U'-unknown(needs to be reviewed)  
`WIDTH` Width limit of the segment (FT), used for routing  
`HEIGHT` Height limit of the segment (FT), used for routing  
`WEIGHT` Weight limit of the segment(LBS), used for routing  
`SPD_LIM` Speed limit of the segment, expressed in MPH, used for routing  
`FCODE` A 2 char representation of allowable values for street classes: HY(highway), EX(expressway), MA(major arterial), MI(minor arterial), CO(collector), RE(residential, neighborhood), AL(alleyway), EA(easement)  
`NAME_FROM` Intersection/street names from  
`NAME_TO` Intersection/street names to  

####SINGLE_STREETS
`PID MASTER_ID` ID of the street name from BAS_STREET_MASTER table  
`PREFIX` Street directional prefix  
`NAME` Street name  
`SUFFIX` follows the name of a street to further describe that street  
`TYPE` Street type abbreviation(Road = Rd, Street = St, Avenue = Ave, Court = Ct, etc)  
`CLASS`  A 2 char representation of allowable values for street classes: HY(highway), EX(expressway), MA(major arterial), MI(minor arterial), CO(collector), RE(residential, neighborhood), AL(alleyway), EA(easement)  
`ROW_WIDTH` Width of right-of-way(international feet)  
`FOC_WIDTH` Distance from top of the curb on one side of the street to the top of the curb on other side of the street  
`ADD_TYPE` The type of address sequences are standard even side-odd side numbering, contiguous numbering such as in a cul-de-sac, other numbering schemes  
`FRADD_L` Address range limitation for the LEFT street side at the starting point of the digitization  
`FRADD_R` Address range limitation for the RIGHT street side at the starting point of the digitization  
`TOADD_L` Address range limitation for the LEFT street side; at the end point of the digitization  
`TOADD_R` Address range limitation for the RIGHT street side at the end point of the digitization  
`MUNI_L` Name of municipality on the left side of the street segment  
`MUNI_R` Name of municipality on the right side of the street segment  
`ZIP_L` Zip-code on the left side of the street segment  
`ZIP_R` Zip-code on the right side of the street segment  
`PRIVATE` A character flag (Y/N) that indicates if the street is private or public  
`ONE_WAY` Contains values for street segment direction flags:'B' -2 way street. 'P'-one way with traffic to the same direction as segment digitized. 'N'-one way with traffic in opposite direction as segment digitized. 'U'-unknown(needs to be reviewed)  
`WIDTH` Width limit of the segment(FT), used for routing  
`HEIGHT` Height limit of the segment(FT), used for routing  
`WEIGHT` Weight limit of the segment(LBS), used for routing  
`SPD_LIM` Speed limit of the segment, expressed in MPH, used for routing  
`FCODE` A 2 char representation of allowable values for street classes: HY(highway), EX(expressway), MA(major arterial), MI(minor arterial), CO(collector), RE(residential, neighborhood), AL(alleyway), EA(easement)  
`NAME_FROM` Intersection/street names from  
`NAME_TO` Intersection/street names to  


### Projections
* GeoJSON, and KMZ files are in WGS84 coordinate system.
* The zipped files are shapefiles in NAD_1983_StatePlane_California_III_FIPS_0403_Feet projected coordinate system.

###Source
City of San Jose - Public Works GIS Team  
200 East Santa Clara Street  
San Jose, CA 95113  
