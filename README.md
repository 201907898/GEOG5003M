# GEOG5003M
Final project for 2026 class GEOG5003M for student 201907898
Context of Project:

Aims of Code: Produce visualizations highlighting patterns between income equality and library usage in Manitoba, Canada in 2021 for an intended audience of 
policy analysts and researchers involved in understanding the relationships between income equality and community resources such as libraries. 

The Gini index on adjusted household after-tax income on the census subdivision level from Census year 2021 will be examined alongside library 
usage metrics from 2021 in Manitoba, and correlations will be assessed.

How were measures of inequality related to library usage in Manitoba in 2021?


Data:

(1) Manitoba library statistics 2021 All library systems including Winnipeg - Membership

• Download name: _temp_published_published_table_report_2388_19386
• Date of download: 12 July, 2026
• Temporal coverage and resolution: Annual data for 2021 including all public libraries in Manitoba.
• Known limitations or quality issues: Nil values entered into dataset as numeric '0'

• Variable Information
 0   Location                                  Name of Library      
 1   Membership as % of Population Served      Percent of population in catchment     
 2   Total Active Library Memberships          Number memberships      
 3   Non-resident, Single memberships          Number memberships   
 4   Non-resident, Family memberships          Number memberships   
 5   Total Non-resident Memberships            Number memberships  
 6   % Memberships Non-resident                Percent of memberships    
 7   Fee for non-resident membership - Single  Canadian Dollar    
 8   Fee for non-resident membership - Family  Canadian Dollar    
 9   Population Served                         Individuals  
 



(2) Manitoba library statistics 2021 -All library systems including Winnipeg - Other Activity
• Download name: _temp_published_published_table_report_2246_19381
• Temporal coverage and resolution: Annual data for 2021 including all public libraries in Manitoba.Date of download: 12 July, 2026
• Known limitations or quality issues: Nil values entered into dataset as numeric '0'

• Variable Information
 0   Location                       Name of Library 
 1   Visits per hour                Annual gate count / hours open in year
 2   Visits per Week                Annual gate count / weeks open in year
 3   Annual Visits per Capita       Annual gate count / population served
 4   Gate Count                     Annual number visitors to library 
 5   Info Transactions per Hour     Annual number transactions / hours open in year
 6   Info Transactions per Week     Annual number transactions / weeks open in year 
 7   Informational Transactions     Annual number transactions 
 8   Computer Bookings per Hour     Annual computer bookings / hours open in year
 9   Computer Bookings per Week     Annual computer bookings / weeks open in year 
 10  Program Attendance             Annual program attendance count
 11  Program Attendance Per Capita  Annual program attendance / population served
 12  Visits to the library website  Annual number of website visitors 
 13  Website visits per Capita      Annual number visits / population served
 14  Population Served              Number of people in library catchment area




(3) List of libraries with census region and exact location

• Download name: ODCAF_V1.0
• Date of download/access: 10 July, 2026
• Temporal coverage and resolution: Data collected between January - July 2020
• Coordinate reference system: EPSG:4326 

• Variable Information
 0   Index                  Index 
 1   Facility_Name          Name of Facility
 2   Source_Facility_Type   Facility type chosen by data provider
 3   ODCAF_Facility_Type    Facility type assigned from nine ODCAF categories
 4   Provider               Name of data provider
 5   Unit                   Civic unit or suite number
 6   Street_No              Civic street number
 7   Street_Name            Civic street name
 8   Postal_Code            Postal Code
 9   City                   Name of City
 10  Prov_Terr              Province or Territory
 11  Source_Format_Address  Full address
 12  CSD_Name               Census subdivision name
 13  CSDUID                 Census Subdivision Unique Identifier
 14  PRUID                  Province Unique Itentifier
 15  Latitude               Latitude of center location
 16  Longitude              Longitude of center location




(4) Census 2021 income inequality measures of Persons in private households in occupied private dwellings
• Download name: 9810096-eng
• Date of download/access: 10 July, 2026
•Temporal coverage: 2016 and 2021 Census data comparison
• Spatial resolution: Canada, Province or territory, Census division, Census subdivision

• Variable information
 0   REF_DATE                 Census year 
 1   GEO                      Name of Location
 2   DGUID                    Dissemination Geography Unique Identifier
 3   Inequality measures (5)  Type of Inequality Measure
									Total Population in private households
									Gini index on adjusted household market income
									Gini index on adjusted household total income
									Gini index on adjusted household after-tax income
									P90/P10 ratio on adjusted household after-tax income
 4   Coordinate               Coordinate
 5   Year (2):2020[1]         Value of inequality measure in 2021 Census
 6   Symbol                   NaN 
 7   Year (2):2015[2]         Value of inequality measure in 2016 Census
 8   Symbol.1                 NaN



(5) Census region shapefile

• Downloaded name: lcsd000a21a_e
• Date of download/access: 10 July, 2026
• Coordinate reference system: EPSG:3347
• Version information: 2021
• Spatial extent and resolution: Major land mass of Canada not including coastal water area
• Processing steps applied: This original file was uploaded to ArcGIS Pro, the 
'Feature Class to Shapefile' geoprocessing tool was used to filter for Manitoba (PRUID = 46),
and the resulting subset of the shapefile was used in analysis.

• Variable information:
 0   CSDUID    Census Subdivision Unique Identifier  
 1   DGUID     Dissemination Geography Unique Identifier 
 2   CSDNAME   Census division name  
 3   CSDTYPE   Census division type  
 4   LANDAREA  Land area  
 5   PRUID     Province Unique Identifier  
 6   geometry  geometry data






References:

I have made no use of generative AI.

(1) Manitoba Sport, Culture, Heritage and Tourism. Manitoba Public Library Statistics : 
Ready Reports 2021 All library systems: Membership. Counting Opinions (SQUIRE) Ltd.
[Online] 2021. [Accessed 12 July, 2026]. Available from:
https://mb.countingopinions.com/pireports/report.php?1e252d64aec50eda2f86aef32e7967f9&live

(2) Manitoba Sport, Culture, Heritage and Tourism. Manitoba Public Library Statistics : 
Ready Reports 2021 All library systems: Other Activity. Counting Opinions (SQUIRE) Ltd.
[Online] 2021. [Accessed 12 July, 2026]. Available from:
https://mb.countingopinions.com/pireports/report.php?5bbe1a6e554a07ad4c016b468bd4e7b8&live

(3) Statistics Canada. The Open Database of Cultural and Art Facilities. Government of Canada. 
[Online]. 2025. [Accessed 10 July 2026]. Available from:
https://www.statcan.gc.ca/en/lode/databases/odcaf

(4) Statistics Canada. Table 98-10-0096-01  Income inequality statistics across Canada: 
Canada, provinces and territories, census divisions and census subdivisions. Government 
of Canada. [Online]. 2022. [Accessed 10 July 2026]. Available from:
https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=9810009601&pickMembers%5B0%5D=1.1

(5) Statistics Canada. 2021 Census – Boundary files. Government of Canada. [Online]. 2023.
[Accessed 10 July 2026]. Available from:
https://www12.statcan.gc.ca/census-recensement/2021/geo/sip-pis/boundary-limites/index2021-eng.cfm?year=21

(6) Matthew Wickline. Coblis — Color Blindness Simulator. Human-Computer Interaction Resource Network.
[Online]. 2001. [Accessed 18 July 2026]. Available from:  
https://www.color-blindness.com/coblis-color-blindness-simulator/
