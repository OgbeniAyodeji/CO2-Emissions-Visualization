# Per capita CO₂ emissions - Data package

This data package contains the data that powers the chart ["Per capita CO₂ emissions"](https://ourworldindata.org/grapher/co-emissions-per-capita?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on March 05, 2025.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


## Annual CO₂ emissions (per capita)
Annual total emissions of carbon dioxide (CO₂), excluding land-use change, measured in tonnes per person.
Last updated: November 21, 2024  
Next update: November 2025  
Date range: 1750–2023  
Unit: tonnes per person  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Global Carbon Budget (2024); Population based on various sources (2024) – with major processing by Our World in Data

#### Full citation
Global Carbon Budget (2024); Population based on various sources (2024) – with major processing by Our World in Data. “Annual CO₂ emissions (per capita) – GCB” [dataset]. Global Carbon Project, “Global Carbon Budget”; Various sources, “Population” [original data].
Source: Global Carbon Budget (2024), Population based on various sources (2024) – with major processing by Our World In Data

### What you should know about this data
* Per capita emissions represent the emissions of an average person in a country or region - they are calculated as the total emissions divided by population.
* This data is based on territorial emissions, which do not account for emissions embedded in traded goods.
* Emissions from international aviation and shipping are not included in any country or region's emissions. They are only included in the global total emissions.

### Sources

#### Global Carbon Project – Global Carbon Budget
Retrieved on: 2024-11-21  
Retrieved from: https://globalcarbonbudget.org/  

#### Various sources – Population
Retrieved on: 2024-07-11  
Retrieved from: https://ourworldindata.org/population-sources  

#### Notes on our processing step for this indicator
- Data on global emissions has been converted from tonnes of carbon to tonnes of carbon dioxide (CO₂) using a conversion factor of 3.664.
- Emissions from the Kuwaiti oil fires in 1991 have been included as part of Kuwait's emissions for that year.
- Country's share of the global population is calculated using our population dataset, based on [different sources](https://ourworldindata.org/population-sources).
- Each country's share of global CO₂ emissions from flaring has been calculated using global CO₂ emissions from flaring provided in the Global Carbon Budget dataset.



    