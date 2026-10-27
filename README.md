# Conservation Crew

## Group members: 1. Gina Givens 2. Jasleen Kalsi 3. Sara Huang 4. Ruixin Yang

Research Question: Are white-tailed deer observations more frequent at a close distance to developed areas that border wildland vegetation in North Carolina?

Target Audience: As white-tailed deer populations in North Carolina increase due to few natural predators and population growth during off-hunting seasons, human-deer conflicts can become more prevalent. This sometimes means an increase in vehicle collisions between the two. Knowing the number of deer and distance they are away from developed areas bordering wildland vegetation can inform the North Carolina Wildlife Resources Commission on region specific harvest strategies. It can also help land owners and land conservation organizations understand where to watch for increased deer presence in their neighborhoods and on protected lands. 

## Data Dictionary- WUI NC Dataset

### Dataset Overview

This dataset represents the Wildland–Urban Interface (WUI) in North Carolina for 1990, 2000, 2010, and 2020. The WUI is the area where houses meet or intermingle with undeveloped wildland vegetation. The dataset combines U.S. Census housing and population data with land-cover information to classify geographic areas by housing density, vegetation, and WUI status.

**Data source:** SILVIS Lab, Department of Forest and Wildlife Ecology, University of Wisconsin–Madison.## Data Source

This analysis uses the North Carolina subset of the
1990–2020 Wildland–Urban Interface (WUI) dataset,
Version 4, produced by SILVIS Lab at the University
of Wisconsin–Madison.

Source: https://silvis.forest.wisc.edu/data/wui-change/

Variable definitions are based on the dataset's
official metadata:
https://geoserver.silvis.forest.wisc.edu/geodata/wui_change_2020_v4/CONUS_WUI_block_1990_2020_change_v4_FGDC_MetadataUpdate.html

**Official dataset:** [The 1990–2020 Wildland–Urban Interface](https://silvis.forest.wisc.edu/data/wui-change/)

**Official metadata:** [SILVIS WUI dataset metadata](https://geoserver.silvis.forest.wisc.edu/geodata/wui_change_2020_v4/CONUS_WUI_block_1990_2020_change_v4_FGDC_MetadataUpdate.html)

### Unit of Observation

Each row represents one mapped polygon feature containing information about housing, population, land cover, and WUI classification. A row represents a geographic area, not an individual person, household, or housing unit.

### Variable Definitions

| Variable | Unit of Measurement | Definition |
|---|---|---|
| `BLK20` | Identifier | Unique identifier associated with 2020 Census block geography. |
| `WATER20` | Flag (1 = water) | Indicates whether the polygon is identified as a water body using 2020 TIGER data. |
| `AWATER20PC` | Percent (%) | Percentage of the block area classified as water. |
| `POP2020` | Persons | Population in 2020. |
| `HU2020` | Housing units | Total housing units in 2020. |
| `OCCHU2020` | Housing units | Occupied housing units in 2020. |
| `VACHU2020` | Housing units | Vacant housing units in 2020. |
| `POPDEN2020` | Persons per square kilometer | Population density in 2020. |
| `HUDEN2020` | Housing units per square kilometer | Total housing-unit density in 2020. |
| `OCCHUDEN20` | Not explicitly specified in the supplied field metadata | Numeric field. The name suggests occupied housing-unit density in 2020, but the supplied metadata does not explicitly define it. |
| `VACHUDEN20` | Not explicitly specified in the supplied field metadata | Numeric field. The name suggests vacant housing-unit density in 2020, but the supplied metadata does not explicitly define it. |
| `PUBFLAG` | Flag (1 = public land) | Indicates whether the polygon is identified as a protected area. |
| `STATE` | Two-letter state abbreviation | State abbreviation associated with the polygon. |
| `HU1990` | Housing units | Total housing units in 1990, allocated to the dataset's geographic framework. |
| `HU2000` | Housing units | Total housing units in 2000, allocated to the dataset's geographic framework. |
| `HU2010` | Housing units | Total housing units in 2010, allocated to the dataset's geographic framework. |
| `HUDEN1990` | Housing units per square kilometer | Housing-unit density in 1990. |
| `HUDEN2000` | Housing units per square kilometer | Housing-unit density in 2000. |
| `HUDEN2010` | Housing units per square kilometer | Housing-unit density in 2010. |
| `VEG1992PC` | Percent (%) | Wildland vegetation percentage in 1992. Wildland vegetation includes forests, grasslands, and wetlands. |
| `VEG2001PC` | Percent (%) | Wildland vegetation percentage in 2001. |
| `VEG2011PC` | Percent (%) | Wildland vegetation percentage in 2011. |
| `VEG2019PC` | Percent (%) | Wildland vegetation percentage in 2019. |
| `WUIFLAG199` | Integer categorical code | WUI status flag for 1990. |
| `WUICLASS19` | Text category | WUI class label for the 1990 classification. |
| `WUIFLAG200` | Integer categorical code | WUI status flag for 2000. |
| `WUICLASS20` | Text category | WUI class label for the 2000 classification. |
| `WUIFLAG201` | Integer categorical code | WUI status flag for 2010. |
| `WUICLASS_1` | Text category | WUI class label associated with the 2010 classification. |
| `WUIFLAG202` | Integer categorical code | WUI status flag for 2020. |
| `WUICLASS_2` | Text category | WUI class label associated with the 2020 classification. |
| `BUFVEG` | Flag (1 = inside, 0 = outside) | Indicates whether the polygon is within a potential interface buffer around qualifying vegetation areas. |
| `Shape_Leng` | Meters (m) | Length of the polygon geometry in the NAD 1983 Albers projected coordinate system. |
| `Shape_Area` | Square meters (m²) | Area of the polygon geometry in the NAD 1983 Albers projected coordinate system. |

### WUI Classification

The dataset classifies polygons by housing density, wildland vegetation, and proximity to qualifying vegetation areas.

- **Intermix WUI:** Polygons with more than 50% wildland vegetation and at least 6.177635 housing units per square kilometer for the relevant year.
- **Interface WUI:** Polygons meeting the minimum housing-density threshold within buffers around qualifying vegetation areas. The processing history describes qualifying areas as having at least 75% wildland vegetation and exceeding 500 hectares, with a buffer distance of 2,414 meters (2.414 km).
- **Wildland vegetation:** Forests, grasslands, and wetlands.

The WUI class fields contain labels describing housing-density and vegetation categories. The supplied field metadata does not include a complete code-to-label lookup table for the WUI flags.

### Coordinate System

The supplied projection metadata identifies the coordinate system as **NAD 1983 Albers**, with meters as its linear unit. Accordingly, polygon length is expressed in meters and polygon area in square meters.

### Documentation Notes

- The supplied DBF attribute table contains 34 fields.
- The source metadata gives conflicting buffer distances: the `BUFVEG` field definition specifies 2.14 km, while the processing history specifies 2,414 meters (2.414 km). This discrepancy is retained rather than assuming one value is correct.
- The supplied metadata does not explicitly define `OCCHUDEN20` or `VACHUDEN20`, nor does it provide a complete WUI flag code lookup table. These details should be confirmed with the data provider if exact definitions are required.

## Data Dictionary- iNaturalist NC Deer Dataset

### Dataset Overview

This dataset contains cleaned deer observation records from iNaturalist for North Carolina, covering the intended study period of 2010–2020. The dataset includes observation identifiers, dates, geographic coordinates, observation quality grades, and coordinate privacy information.

**Data source:** iNaturalist.

## Data Source

This analysis uses the cleaned North Carolina deer observation dataset, `NC_Deer_Cleaned_2010_2020.csv`.

**Official terminology:** [iNaturalist Terminology](https://www.inaturalist.org/terminology)

Variable definitions are based on the official iNaturalist terminology where available. Fields not explicitly defined in the supplied documentation are described according to their role in the cleaned dataset.

### Unit of Observation

Each row represents one iNaturalist observation record included in the cleaned dataset. A row represents an observation, not necessarily a unique individual deer.

### Variable Definitions

| Variable | Unit of Measurement | Definition |
|---|---|---|
| `id` | Unique identifier | Identifier associated with the iNaturalist observation. |
| `observed_on` | Date | Date on which the observation occurred. |
| `year` | Calendar year | Year associated with the observation date. |
| `time_observed_at` | Date and time | Date and time associated with the observation. |
| `latitude` | Decimal degrees | Latitude coordinate associated with the observation location. |
| `longitude` | Decimal degrees | Longitude coordinate associated with the observation location. |
| `quality_grade` | Categorical | iNaturalist quality classification for the observation, such as `research` or `needs_id`. |
| `coordinates_obscured` | Boolean (`TRUE`/`FALSE`) | Indicates whether the observation's coordinates have been obscured. |

### Observation Quality

The `quality_grade` variable describes the quality classification assigned to an observation by iNaturalist.

- **Research:** An observation classified as research grade by iNaturalist.
- **Needs ID:** An observation classified as needing further identification.

These categories describe the observation's quality status and do not, by themselves, establish that every record has been independently verified.

### Geographic Coordinates

The `latitude` and `longitude` variables describe the geographic location associated with each observation.

- **Latitude:** North–south geographic position, expressed in decimal degrees.
- **Longitude:** East–west geographic position, expressed in decimal degrees.
- **Coordinate privacy:** The `coordinates_obscured` field indicates whether the observation's coordinates have been obscured. Publicly displayed coordinates may not show the exact observation location.

### Documentation Notes

- The supplied CSV contains eight variables.
- The filename indicates an intended study period of 2010–2020, but the filename alone does not confirm that every record falls within this period.
- The `year` variable is described according to its role in the cleaned dataset; the supplied iNaturalist terminology page does not specify how this field was created.
- The precise format and time-zone handling of `time_observed_at` should be confirmed from the original export or data-processing steps if needed.
- Variable definitions follow the [official iNaturalist terminology documentation](https://www.inaturalist.org/terminology) where supported. Definitions inferred from the cleaned dataset are not presented as direct definitions from iNaturalist.

### WUI Data Access and Reproducibility

The Wildland–Urban Interface (WUI) dataset is produced by SILVIS Lab at the University of Wisconsin–Madison. Our group accessed the dataset through the shared Duke Box Drive provided for this class. The original dataset is too large to store in this GitHub repository.

**Official dataset download:** https://silvis.forest.wisc.edu/data/wui-change/

**Dataset metadata:** https://geoserver.silvis.forest.wisc.edu/geodata/wui_change_2020_v4/CONUS_WUI_block_1990_2020_change_v4_FGDC_MetadataUpdate.html

Students in the class can check the shared Duke Box Drive for the dataset. Alternatively, the North Carolina data can be obtained from the official 1990–2020 WUI Change Version 4 dataset.

The existing spatial processing script expects a shapefile named `NC_wui_block_1990_2020_change_v4.shp` in `data/raw_large/`. Keep the shapefile and its associated files together in that directory.

The spatial processing workflow is documented in `Scripts/Spacial Data Quality Audit.Rmd`. Reproducing its output requires access to the WUI source data and the R packages used by the script. Input and output paths may need to be adapted for the local computer before the script can run successfully.

### iNaturalist Deer Data: Reproducibility

The original iNaturalist white-tailed deer observations are stored in `data/raw/NC_WhiteTailedDeer_iNaturalist_public.csv`.

The script `Scripts/02_Deer_Data_Quality_Audit.Rmd` imports the original dataset, assesses data quality, filters observations to dates from January 1, 2010, through December 31, 2020, and selects eight variables for the cleaned dataset: `id`, `observed_on`, `year`, `time_observed_at`, `latitude`, `longitude`, `quality_grade`, and `coordinates_obscured`.

Running the code chunks in the script in order creates the processed dataset at `data/processed/NC_Deer_Cleaned_2010_2020.csv`.

The workflow uses the `readr` R package. The original dataset is kept separate from the processed output. Each row represents an iNaturalist observation, not necessarily a unique individual deer.