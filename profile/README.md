## Identifying Priority Survey Sites for Early-Season Milkweed Conservation

<img width="1400" alt="MilkweedMod_Pres" src="https://github.com/MEDS-SBBG-milkweed/.github/assets/98177666/6049f3c0-e73d-4f78-96f1-634a912ab470">

## Description
Monarch butterfly (Danaus plexippus) populations are experiencing decline due to habitat degradation and climate threats. In 2024, this iconic species became protected under the Endangered Species Act. Critical to the persistence of this species of cultural and ecological importance is milkweed (Asclepias spp.), which monarchs rely on as an essential resource for food and reproduction. Motivated by concerns over the loss of monarch habitat, the Santa Barbara Botanic Garden (SBBG) and local collaborators are working to identify potential restoration areas in the Los Padres National Forest (LPNF). However, the vast size and complex terrain of the LPNF poses a logistical challenge to surveying. Therefore, there is a need for a tool to aid in selecting sites to prioritize. Our team created a priority index for surveying milkweed within the LPNF by predicting the habitat suitability for four early-season milkweed species using Maximum Entropy (MaxEnt) species distribution modeling and creating a novel survey site accessibility index. We identified high-priority sites for the team to survey based on high predicted suitability for each species of early-season milkweed and high physical accessibility. To communicate these results, we created an interactive web dashboard, which the SBBG team will use for field planning to support the ongoing monitoring of milkweed populations for monarch habitat restoration efforts within the LPNF. 

### To achieve this goal we have identified the following objectives:
1. Identify high-priority milkweed survey sites, based on habitat suitability and physical accessibility, throughout the Los Padres National Forest to direct Santa Barbara Botanic Garden summer 2024 field surveys.
   - [milkweed-mod](https://github.com/milkweed-mod/milkweed-mod)

2. Deliver all components of objective 1 in the form of an interactive web dashboard to facilitate field survey planning and allow for future updates as additional data is collected.
   - [milkweed-site-finder](https://github.com/milkweed-mod/milkweed-site-finder)
  
### Data sources

| Data                                                                                                                                             | Source                                                                                                                                | Use                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|
| **SBBG Milkweed Survey Locations (2023 Survey):** milkweed species, presence/absence, location, number of plants (.shp)                | Dr. Sarah Cusser (SBBG) via Google Drive                                                                                              | Habitat Suitability Map, Interactive Web Dashboard                                                              |
| **Bioclim (19 variables):** annual trends, seasonality, extreme/limiting environmental factors based on monthly temperature and rainfall data (.tif) | WordClim via {wallace}’s envs_worldclim() function, which utilizes {raster}’s getData() function in R | Habitat Suitability Map, Survey Site Priority Index, Interactive Web Dashboard                                  |
| **California Multi-Source Land Ownership:** classification of public and private land in the LPNF and surrounding areas (.shp)                       | California Department of Forestry and Fire Protection; California State Geoportal, hosted on CAL FIRE Portal (via gis.data.ca.gov)    | Survey Site Accessibility Index, Survey Site Priority Index                                                     |
| **Canopy Cover:** horizontal cover fraction occupied by tree canopies (.tif)                                                                         | California Forest Observatory, selecting “Canopy Cover” from available datasets to download                                           | Habitat Suitability Map, Survey Site Accessibility Index, Survey Site Priority Index, Interactive Web Dashboard |
| **Digital Elevation Model (DEM):** topographic surface of the earth and flattened water surfaces (.tif)                                              | USGS’s The National Map (TNM) download interface; Elevation Products (3DEP) 1 arc-second DEM                                          | Habitat Suitability Map, Survey Site Accessibility Index, Survey Site Priority Index, Interactive Web Dashboard |
| **Los Padres National Forest (LPNF) Boundary:** boundaries of the northern and southern regions of the LPNF (.gdb)                                   | California State Parks GIS Data (via parks.ca.gov) ESRI geodatabase                                                                   | Habitat Suitability Map,  Survey Site Accessibility Index,  Interactive Web Dashboard                           |
| **LPNF 2023 Trails and Roads:** trails and roads in the southern region of the LPNF (.shp)                                                           | Los Padres Forest Watch via ArcGIS                                                                                                    | Survey Site Accessibility Index,  Survey Site Priority Index, Interactive Web Dashboard                         |
| **USGS 2024 Trails and Roads:** trails and different types of roads in California (.shp), used data from within the northern region of the LPNF      | National Transportation Data (NTD) California Shapefile, courtesy of the U.S. Geological Survey                                       | Survey Site Accessibility Index, Survey Site Priority Index, Interactive Web Dashboard                          |


## Authors and Contributors
 - Amanda Herbst { [Github](https://github.com/amandaherbst) | [Website](amandaherbst.github.io) | [LinkedIn](https://www.linkedin.com/in/amanda-herbst/) }
 
 - Sam Muir { [Github](https://github.com/shmuir) | [Website](https://shmuir.github.io/) | [LinkedIn](https://www.linkedin.com/in/shmuir/) }

 - Anna Ramji { [Github](https://github.com/annaramji) | [Website](https://annaramji.github.io/) | [LinkedIn](https://www.linkedin.com/in/annaramji/) }

 - Melissa Widas { [Github](https://github.com/mwidas) | [Website](https://mwidas.github.io/) | [LinkedIn](https://www.linkedin.com/in/mwidas/) }

### Client 

Dr. Sarah Cusser, Terrestrial Invertebrate Conservation Ecologist <br>
Santa Barbara Botanic Garden <br>
1212 Mission Canyon Rd. <br>
Santa Barbara, CA 93105



