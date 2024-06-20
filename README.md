# Nebraska Election Shapefile

This shapefile was processed by Professor Ellen Veomett and her student Ananya Agarwal.

# **Sources**

Obtain the following data from Restricting Data Hub

[Population data](https://redistrictingdatahub.org/dataset/Nebraska-block-pl-94171-2020-by-table/): based on the decennial census at the Census Block level on 2020 Census Redistricting Data

[Congressional District data](https://redistrictingdatahub.org/dataset/2021-Nebraska-congressional-districts/): 2021 Nebraska Congressional Districts plan enacted on 11/24/21

[State Senate District data](https://redistrictingdatahub.org/dataset/2021-nebraska-state-legislature-adopted-plan/): 2021 State Senate Approved Plan

[2020 election data](https://redistrictingdatahub.org/dataset/vest-2020-nebraska-precinct-boundaries-and-election-results/)**:**  VEST 2020 Nebraska precinct and election results

[2018 election data](https://redistrictingdatahub.org/dataset/vest-2018-nebraska-precinct-and-election-results/)**:**  VEST 2018 Nebraska precinct and election results

[2016 election data](https://redistrictingdatahub.org/dataset/vest-2016-nebraska-precinct-and-election-results/)**:**  VEST 2016 Nebraska precinct and election results

## Processing
Some merging of precincts in the tabular election data and precinct shapefile were necessary to join election results to precinct boundaries. Data from absentee votes reported at the county level were disaggregated to precincts by voting age population. Demographic data were aggregated from blocks to precincts using MGGG’s proration software. Congressional and state legislative district IDs were also assigned to precincts using this package.

## Metadata
* `STATE`: State
* `STATEFP`: State FIPS code
* `COUNTY`: County name
* `COUNTYFP`: County FIPS code
* `Precinct`: Precinct name
* `CODE`: Precinct code
* `GOV18D`: Number of votes for 2018 Democratic gubernatorial candidate, without absentee votes
* `GOV18R`: Number of votes for 2018 Republican gubernatorial candidate, without absentee votes
*	`USH18D`: Number of votes for 2018 Democratic US House candidate, without absentee votes
*	`USH18R`: Number of votes for 2018 Republican US House candidate, without absentee votes
*	`SOS18D`: Number of votes for 2018 Democratic secretary of state candidate, without absentee votes
*	`SOS18R`: Number of votes for 2018 Republican secreatary of state candidate, without absentee votes
* `GOV18D+`: Number of votes for 2018 Democratic gubernatorial candidate, with absentee votes
* `GOV18R+`: Number of votes for 2018 Republican gubernatorial candidate, with absentee votes
*	`USH18D+`: Number of votes for 2018 Democratic US House candidate, with absentee votes
*	`USH18R+`: Number of votes for 2018 Republican US House candidate, with absentee votes
*	`SOS18D+`: Number of votes for 2018 Democratic secretary of state candidate, with absentee votes
*	`SOS18R+`: Number of votes for 2018 Republican secreatary of state candidate, with absentee votes
* `TOTPOP`: Total population from 2010 Decennial Census
* `NH_WHITE`: White, non-hispanic, population from 2010 Decennial Census
* `NH_BLACK`: Black, non-hispanic, population from 2010 Decennial Census
* `NH_AMIN`: American Indian and Alaska Native, non-hispanic, population from 2010 Decennial Census
* `NH_ASIAN`: Asian, non-hispanic, population from 2010 Decennial Census
* `NH_NHPI`: Native Hawaiian and Pacific Islander, non-hispanic, population from 2010 Decennial Census
* `NH_OTHER`: Other race, non-hispanic, population from 2010 Decennial Census
* `NH_2MORE`: Two or more races, non-hispanic, population from 2010 Decennial Census
* `HISP`: Hispanic population from 2010 Decennial Census
* `H_WHITE`: White, hispanic, population from 2010 Decennial Census
* `H_BLACK`: Black, hispanic, population from 2010 Decennial Census
* `H_AMIN`: American Indian and Alaska Native, hispanic, population from 2010 Decennial Census
* `H_ASIAN`: Asian, hispanic, population from 2010 Decennial Census
* `H_NHPI`: Native Hawaiian and Pacific Islander, hispanic, population from 2010 Decennial Census
* `H_OTHER`: Other race, hispanic, population from 2010 Decennial Census
* `H_2MORE`: Two or more races, hispanic, population from 2010 Decennial Census
* `VAP`: Total voting age population from 2010 Decennial Census
* `HVAP`: Hispanic voting age population from 2010 Decennial Census
* `WVAP`: White, non-hispanic, voting age population from 2010 Decennial Census
* `BVAP`: Black, non-hispanic, voting age population from 2010 Decennial Census
* `AMINVAP`: American Indian and Alaska Native, non-hispanic, voting age population from 2010 Decennial Census
* `ASIANVAP`: Asian, non-hispanic, voting age population from 2010 Decennial Census
* `NHPIVAP`: Native Hawaiian and Pacific Islander, non-hispanic, voting age population from 2010 Decennial Census
* `OTHERVAP`: Other race, non-hispanic, voting age population from 2010 Decennial Census
* `2MOREVAP`: Two or more races, non-hispanic, voting age population from 2010 Decennial Census
* `CD`: Congressional district
* `SEND`: State Senate district

Notes: State house districts are not included because Nebraska has a unicameral legislature. Also, the Nebraska governor and lieutenant governor are elected together, so the gubernatorial results also represent lieutenant governor results.

## Projection
This shapefile uses a Lambert Conformal Conic/State Plane projection centered on Nebraska (ESPG:6516).
