# Scripts for project

For all these scripts, it is assuming it is being ran under Google Cloud Platform. They all use PySpark in Google Dataproc. Data extraction was done through the Linux command line in a compute instance, which is why it is not a script. 

Below are quick descriptions on what each script does.

## EDA
Performs exploratory data analysis upon the raw data.

## CleanData
Reads raw data from the bucket and cleans it. Then, it writes the clean data back into a bucket.

## ModelCreation
Reads clean data and trains a linear regression model using a cross validator. It then saves the transformed data it used for model training as well as the model it created back into the bucket.

## Model Visualization
Creates visualizations with the newly created model and saves them as png's. 
