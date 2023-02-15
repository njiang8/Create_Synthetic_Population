# Create Synthetic Population

This project contains all functions that create synthetic population in NY, NJ, CT, and PA areas (as the figure shown). 
<p align="center">
  
  <img  src="https://github.com/njiang8/Create_Synthetic_Population/blob/master/Study_Area.png">

 </p>

Our methods use open-source data as the input to generate synthetic population as the table shown below. If the following links are no longer valid, the data can be found in https://osf.io/3vsaj/ under the input folder. The results files can be found under the output folder.

|      Type     |     Dataset   | Source |
| ------------- | ------------- | ------------ |
| Raod Network | 2010 U.S. Census TIGER Shapefiles  | https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2010&layergroup=Roads |
|  Population  | 2010 U.S. Census Tracts  | https://www.census.gov/programs-surveys/geography.html |
|  Education   |US Environmental Protection Agency (EPA) Office of Environmental Information (OEI) | https://edg.epa.gov/metadata/catalog/search/resource/details.page?uuid=%7B9C49AE4B-F175-43D0-BCC6-A928FF54C329%7D |
|  Workplace   |2010 U.S. Census Bureau’s County Business Patterns | https://lehd.ces.census.gov/data/lodes/LODES7/ |


Our method includes the following steps:
* [Step 1](https://github.com/njiang8/Create_Synthetic_Population/blob/master/0_Data_Preprocessing.ipynb). Data preprocessing, clean raod network and commute infomation
* [Step 2](https://github.com/njiang8/Create_Synthetic_Population/blob/master/1_Creat_Individuals.ipynb).	Generating workplaces, individual agents organized into households and place workplaces and  individuals on the cleaned road lines. 
* [Step 3a](https://github.com/njiang8/Create_Synthetic_Population/blob/master/2_Assign_Kids_School_Daycare_Unique_IDs.ipynb).	Assigning individual agents to their daytime locations including work, school and daycare
* [Step 3b](https://github.com/njiang8/Create_Synthetic_Population/blob/master/3_Assign%20RID.ipynb).  Assigning unique Road ID (extracted from road line) to individual agents, work loactions, school and daycare.
* [Step 4](https://github.com/njiang8/Create_Synthetic_Population/blob/master/4_Create_Networks.ipynb).	Creating individual networks representing group membership in a family or other household type and either a work or school

Realted Publication
https://link.springer.com/article/10.1007/s43762-022-00034-1

This project is supported by the Center for Social Complexity at George Mason University and the Defense Threat Reduction Agency (DTRA) under Grant number HDTRA1-16-0043. The opinions, findings, conclusions or recommendations expressed in this work are those of the researchers and do not necessarily reflect the views of the sponsors.

**You may find a file called "How to run the code" to replicate the genrataion process.**
