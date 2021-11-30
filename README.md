# train-prediction-project

## How to use:

1. Open the file [data_analysis_prediction.ipynb](https://github.com/adrian-ja-projects/train-prediction-project/blob/main/data_analysis_train_prediction.ipynb)
2. Click on the Google colab logo in the file.
3. Run all the cells. It should take around 3 mins to run all.
4. Get the recommendation done by the data analysis in the last cell of the notebook.
5. In the notebook, ff you click the folder icon on the left side bar, you will see all the data extract in multiple data zones.

## What is doing:

This programme is using google colabs notebooks as environment to reduce dependency risks. 
1. Extract data from the digitraffic API.
2. Stage the data in an staging folder. 
3. Read the JSON file and automatically flatten the file.
4. Write the flat file into a parquet table in the RAW zone. (original design was to upload the file into a DB, time contrains change the design to write into data lake format)
5. Read the parquet table and transform to get the table ready for analysis. Write table into a Use Case area (Golden Area)
6. Analysis is carried out to get a suggested maximun departing time for the IC27 train.
