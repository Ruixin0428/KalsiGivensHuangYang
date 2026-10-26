# Data Metadata

## Dataset Name
North Carolina Wildland-Urban Interface (WUI), 1990–2020

## Dataset Description
Data Metadata

Dataset Name

North Carolina Wildland-Urban Interface (WUI), 1990–2020

Dataset Description

This dataset contains geospatial data describing the wildland-urban interface (WUI) in North Carolina from 1990 to 2020. The WUI refers to areas where housing meets or intermingles with undeveloped wildland vegetation. The dataset is designed to support research on wildland fire, housing growth, and related policy questions.

The data are based on U.S. Census housing information and National Land Cover Database (NLCD) vegetation data. The North Carolina dataset represents geographic areas based on Census blocks and includes information about housing, population, vegetation, and WUI classifications over time.

Data Source

SILVIS Lab, Department of Forest and Wildlife Ecology, University of Wisconsin–Madison.

Dataset title in the source metadata: The 1990–2020 Wildland-Urban Interface of the Conterminous United States (Version 4) — Geospatial Data.

Source website: http://silvis.forest.wisc.edu/housing/block_change

Temporal Coverage

The dataset covers 1990–2020, with WUI and housing information for 1990, 2000, 2010, and 2020. Vegetation attributes reference land-cover data from 1992, 2001, 2011, and 2019.

Spatial Coverage and Format

Geographic coverage: North Carolina, United States.

Geometry: Polygons representing geographic areas based on Census blocks.

Coordinate reference system: NAD 1983 Albers.

File format: ESRI Shapefile, consisting of multiple related files, including .shp, .shx, .dbf, and .prj.

Expected Variables

The source metadata lists variables related to the following categories:

Geographic identifiers: BLK20, STATE

Population and housing: POP2020, HU2020, OCCHU2020, VACHU2020, HU1990, HU2000, HU2010

Housing and population density: POPDEN2020, HUDEN2020, OCCHUDEN20, VACHUDEN20, HUDEN1990, HUDEN2000, HUDEN2010

Water coverage: WATER20, AWATER20PC

Vegetation coverage: VEG1992PC, VEG2001PC, VEG2011PC, VEG2019PC

WUI classification and flags: fields with names beginning WUIFLAG and WUICLASS

Other attributes: PUBFLAG, BUFVEG, Shape_Leng, Shape_Area

These are variable names listed in the source metadata. Exact field names and definitions should be checked against the actual shapefile attribute table before analysis.

Access and Storage

The dataset is available through the course team's shared Box folder. Team members should use the North Carolina dataset folder or its ZIP archive, NC_wui_block_1990_2020_change_v4_shp.zip.

Because the dataset is large, it should not be committed to GitHub. Team members using the RStudio container should upload their own copy into data/raw/raw_large/, following the course instructions. The .gitignore file excludes files in this folder from Git tracking.

Shared Box folder: https://duke.box.com/s/6bw5buacqwfsa9ih0pqg6rfzaxfhwg8m

Team members should verify that they have permission to access and download the North Carolina dataset from Box before attempting to reproduce the analysis.

Permissions and Restrictions

The source metadata lists no specific restrictions and states that acknowledgment of the USDA Forest Service Northern Research Station in products, presentations, and publications using the data would be appreciated. The metadata also states that the data providers make no warranty regarding the data.

Recommended acknowledgment: USDA Forest Service Northern Research Station.

References

SILVIS Lab, University of Wisconsin–Madison: http://silvis.forest.wisc.edu/housing/block_change

Multi-Resolution Land Characteristics Consortium, National Land Cover Database: https://www.mrlc.gov/data/nlcd-land-cover-conus-all-years

U.S. Geological Survey, NLCD data: https://doi.org/10.5066/P9KZCM54