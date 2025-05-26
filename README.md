# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)

Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.

See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

## DATA & FILE OVERVIEW

The data folder, `data/`, contains two folders: raw/ and processed/. The structure of the data folder is as follows:

```bash
data
├── processed
│   ├── all_cover_fixed_LIZPETERSON.csv
│   ├── snow_cover.csv
│   └── species_presence.csv
├── raw
│   ├── 01_ASDN_Readme.txt
│   ├── ASDN_Daily_species.csv
└── └── ASDN_Snow_survey
```
- `all_cover_fixed_LIZPETERSON.csv`: Cleaned snow survey data
- `snow_cover.csv`: Partially cleaned snow cover survey data (only the `snow_cover` column was cleaned)
- `species_presence.csv`: Cleaned species data
- `01_ASDN_Readme.txt`: Original metadata from ASDN
- `ASDN_Daily_species.csv`: Species survey data from ASDN
- `ASDN_Snow_survey`: Snow cover survey data from ASDN

#### Additional related data collected that was not included in the current data package:
- ASDN_Invert_biomass.csv
- ASDN_Bird_sexes.csv
- ASDN_Weather_Hobo.csv
- ASDN_Bird_nests.csv
- ASDN_Pred_nests.csv
- ASDN_Camp_staff.csv
- ASDN_Weather_snow_manual.csv
- ASDN_Weather_precip_manual.csv
- ASDN_Pred_point_counts.csv
- ASDN_Daily_species_effort.csv
- ASDN_Lemming_trap.csv
- ASDN_Camp_info.csv
- ASDN_Lemming_nests.csv
- ASDN_Daily_pred_lemm.csv
- ASDN_Bird_captures.csv
- ASDN_Surface_water.csv
- ASDN_Geodata.csv
- ASDN_Bird_eggs.csv
- ASDN_Lemming_counts.csv
- ASDN_Bird_resights.csv

5. Are there multiple versions of the dataset? 
The version of the dataset that we use was created for the EDS 213 course at the Bren School of Environmental Science and Management. This is not the original dataset from ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W).

## DATA-SPECIFIC INFORMATION FOR:

For the file `data/processed/all_cover_fixed_LIZPETERSON.csv` : 

1. Number of variables: 11

2. Number of cases/rows: 42,830


| Variable name | Description                                                                                                                                                           | Unit(s) / Value type |
|---------------|------------------------------------------------------------|----------------------|
| Site          | Four-letter code of site at which data were collected                                                                                                                 | string               |
| Year          | Year in which data were collected                                                                                                                                     | integer              |
| Date          | Date on which data were collected                                                                                                                                     | date                 |
| Plot          | Name of study plot on which survey was conducted                                                                                                                      | string               |
| Location      | Name of dedicated snow-survey location, if applicable                                                                                                                 | string               |
| Snow_cover    | Percent cover of snow, including slush                                                                                                                                | integer              |
| Water_cover   | Percent cover of water                                                                                                                                                | integer              |
| Land_cover    | Percent cover of exposed land                                                                                                                                         | integer              |
| Total_cover   | Sum of the three cover columns - they should sum to 100%. | integer              |
| Observer      | Person who conducted the survey                                                                                                                                       | string               |
| Notes         | Any relevant comments on the survey                                                                                                                                   | string               |

5. Missing data codes: NA

6. Specialized formats or other abbreviations used:


## SHARING/ACCESS INFORMATION

1. Licenses/restrictions placed on the data:

2. Links to publications that cite or use the data:

3. Links to other publicly accessible locations of the data:

4. Links/relationships to ancillary data sets: <any supplementary data sources 
that support analysis or classification of the datasets, eg., plant taxonomy table.)>

5. Was data derived from another source? If yes, list source(s): <list citations 
to original sources>

6. Recommended citation for the project:
The ASDN metadata 
Please acknowledge this dataset and the authors in any analysis, publication, presentation, or other output that uses these data. If you use the full dataset, we suggest you cite it as:

Lanctot, RB, SC Brown, and BK Sandercock. 2016. Arctic Shorebird Demographics Network. NSF Arctic Data Center. doi: INSERT HERE.

If you use data from only one or a few sites, we suggest you cite data for each site as per this example, using the corresponding site PIs as the authors:

Lanctot, RB and ST Saalfeld. 2016. Barrow, 2014. Arctic Shorebird Demographics Network. NSF Arctic Data Center. doi: INSERT HERE.

Note that each updated version of the full dataset has its own unique DOI.
