# Create_Synthetic_Population

This project contains all functions that creates synthetic popultion in NY, NJ, CT and PA area. Our methods use open-source data to generate the synthetic popultion as the table shown below.

|      Type     |     Dataset   | Source |
| ------------- | ------------- | ------------ |
| Raod Network | 2010 U.S. Census TIGER Shapefiles  | https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2010&layergroup=Roads |
|  Population  | 2010 U.S. Census Tracts  | https://www.census.gov/programs-surveys/geography.html |
|  Education   |US Environmental Protection Agency (EPA) Office of Environmental Information (OEI) | https://edg.epa.gov/metadata/catalog/search/resource/details.page?uuid=%7B9C49AE4B-F175-43D0-BCC6-A928FF54C329%7D |
|  Workplace   |2010 U.S. Census Bureau’s County Business Patterns | https://lehd.ces.census.gov/data/lodes/LODES7/ |


Our method includes the following steps:
1.	Generating individual agents organized into households and place them on the cleaned road lines
2.	Assigning individual agents to their daytime locations including work, school and daycare
3.  Assigning unique Road ID (extracted from road line) to individual agents, work loactions, school and daycare.
4.	Creating individual networks representing group membership in a family or other household type and either a work or school

