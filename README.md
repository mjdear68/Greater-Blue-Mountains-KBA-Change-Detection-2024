# BirdLife Australia Key Biodiversity Area (KBA) Change Detection

The purpose of this project is to identify change in land cover for a given KBA using a classification based on NDVI thresholds.

## Method
Sentinel 2 satellite data is obtained from [Digital Earth Australia's](https://www.dea.ga.gov.au/) Open Data Cube for selected months in each year for the current year and the previous five years. Each hectare in the study area is represented by one pixel in the dataset. NDVI and a 5-year mean datasets are produced. True-colour (RGB) and NDVI images of the KBA and its surrounds are plotted for manual review. A classification is developed using NDVI thresholds, from which class change matrices are produced.

## Usage
1. Run the Data Extraction notebook from within the [Digital Earth Australia Sandbox](https://app.sandbox.dea.ga.gov.au/).
2. Run the Analysis notebook. This can be performed locally by first downloading the two `.nc` files exported from the Data Extraction notebook, or from within the [Digital Earth Australia Sandbox](https://app.sandbox.dea.ga.gov.au/).

## Recommendations
* The BirdLife Australia KBA reporting period is Easter to Easter in consecutive years.
* To reduce the amount of data and to make comparisons at approximately the same time each year, it is recommended that data be selected from January to March of each year.

## References
The notebooks are based on the following DEA notebooks:
* [Parallel Processing With Dask Beginner's Guide](https://knowledge.dea.ga.gov.au/notebooks/Beginners_guide/09_Parallel_processing_with_Dask/)
* [Calculating Band Indices How-to](https://knowledge.dea.ga.gov.au/notebooks/How_to_guides/Calculating_band_indices/)
* [Generating Composite Images How-to](https://knowledge.dea.ga.gov.au/notebooks/How_to_guides/Generating_composites/)
* [Extract and Analyse Data for Multiple Polygons](https://knowledge.dea.ga.gov.au/notebooks/How_to_guides/Analyse_multiple_polygons/)