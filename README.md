# Data Processing from French Census Data for multi-year scenario

This git is an adaptation from [this git](https://github.com/vdarsel/French_Census_Data_Processing). This adaptation aims to propose a dataset that aligns characteristics between years. In particular, some definitions of modalities evolve in time what is taken into account in this depo. Moreover, the geographical codes also evolve in time. We add a correction to align with the last year of data avaialable: 2021.


To run the data processing, initial datasets should be downloaded (see later), then run the following command:
```
python data_process.py

```

This includes data processing (data_process.py), correction for multiyear geographical elements (geographical_alignment.py) and split in different training and testing sets (split_population.py). The generated datasets are saved in Generated_data/Census_data_YEAR


## Initial datasets
This Git repository describes the processing from the French Census data, described in [ADD REF WHEN AVAILABLE]. The datasets are derived from the French Institute for Statistics (INSEE), using the Census data from 2007 to 2021.


| Year | Link                                                          |
|------|---------------------------------------------------------------|
| 2007 | https://www.insee.fr/fr/statistiques/2408061?sommaire=2408480 |
| 2008 | https://www.insee.fr/fr/statistiques/2408667?sommaire=2409062 |
| 2009 | https://www.insee.fr/fr/statistiques/2411383                  |
| 2010 | https://www.insee.fr/fr/statistiques/2411430?sommaire=2411542 |
| 2011 | https://www.insee.fr/fr/statistiques/2011208?sommaire=2011338 |
| 2012 | https://www.insee.fr/fr/statistiques/1913195                  |
| 2013 | https://www.insee.fr/fr/statistiques/2409376                  |
| 2014 | https://www.insee.fr/fr/statistiques/3141862?sommaire=2866354 |
| 2015 | https://www.insee.fr/fr/statistiques/3625223?sommaire=3558417 |
| 2016 | https://www.insee.fr/fr/statistiques/4229118?sommaire=4171558 |
| 2017 | https://www.insee.fr/fr/statistiques/4802064?sommaire=4508161 |
| 2018 | https://www.insee.fr/fr/statistiques/5542859?sommaire=5395764 |
| 2019 | https://www.insee.fr/fr/statistiques/6544333                  |
| 2020 | https://www.insee.fr/fr/statistiques/7706119?sommaire=7637890 |
| 2021 | https://www.insee.fr/fr/statistiques/8268848                  |

For each link, the data from Zone A corresponding to Île de France should be downloaded in format csv, when possible, or txt. Then, the datasets should be set in the corresponding folder in Data/Raw_census_data_YEAR.

## Variables 

Here is the list of the variables (some were deleted from the one year case).

- Age
- Sex
- Diploma
- isMarried
- Cohabitation
- Employment
- Socioprofessional
- Activity
- Hours
- Transport
- ReferenceLink
- FamilyLink
- HouseholdSize
- nChildren
- nRooms
- Surface
- Parking
- nCars
- Accommodation
- Household
- Occupancy
- Department
- County
- City
