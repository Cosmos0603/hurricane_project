# County-Level Analysis of Hurricane Impacts on Consumption Patterns Across the U.S.

## Datasets
FEMA National Risk Index Dataset:
* provides county level statistics and scores on social vulnerability, hurricane records, hurricane exposure, and hurricane risk
* publically available at https://arcg.is/0KD9Tq

Nielsen Scanner Consumption Dataset:
* provides weekly product sales by county across all states
* not publically available

Census Bureau Dataset:
* provides county level demographical information
* publically available at https://data.world/bdill/county-level-population-by-race-ethnicity-2010-2019

Hurricane Marker CSV:
* provides the markers for past hurricane occurrences
* not publically available

## Notebooks Description
* exploredata_FEMA: explore and preprocess the FEMA data
* exploredata_psid: explore and preprocess the psid data
* exploredata_Nielsen: explore and preprocess the Nielsen data
* exploredata_Census: explore and preprocess the Census data (demo info)
* explore_visualize_data.ipynb: Data Visualizations
* hurricane_marker: explore and preprocess the hurricane_marker.csv
* merge_plot: 
	* merge all the preprocessed data into one single data frames
	* visualize the resulted data frame
* baseline:
	* prepare the data for model training
	* experiment with different baseline models
	* perform county filtering and product grouping
* Model Evaluation: 
	* can be run with the sample data (df_tx_sample.pkl)
	* parameter tuning with randomized search
	* evaluating different models with different feature combinations
