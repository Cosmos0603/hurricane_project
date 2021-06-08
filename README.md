# County-Level Analysis of Hurricane Impacts on Consumption Patterns Across the U.S.

## Datasets
FEMA National Risk Index Dataset:
* provides county level statistics and scores on social vulnerability, hurricane records, hurricane exposure, and hurricane risk
* publically available at https://arcg.is/0KD9Tq

Nielsen Scanner Consumption Dataset:
* provides weekly product sales by county across all states
* not publically available

Hurricane Marker CSV:
* provides the markers for past hurricane occurrences
* not publically available

## Notebooks Description
* exploredata_FEMA: explore and preprocess the FEMA data
* exploredata_psid: explore and preprocess the psid data
* exploredata_Nielsen: explore and preprocess the Nielsen data
* hurricane_marker: explore and preprocess the hurricane_marker.csv
* merge_plot: 
	* merge all the preprocessed data into one single data frames
	* visualize the resulted data frame
* baseline:
	* prepare the data for model training
	* experiment with different baseline models
	* perform county filtering and product grouping
* Model Evaluation: 
	* can be run with the sample data (df_tx_data3.pkl)
	* parameter tuning with randomized search
	* evaluating different models with different feature combinations