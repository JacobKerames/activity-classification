# Activity Classification Model

<img src="https://user-images.githubusercontent.com/108101472/209432584-311c4ce0-61c6-4bef-be80-5ddf492a381c.png" width="1000">

This project involves the creation of an activity classification model that detects hand movement or lack thereof using raw motion data from an Apple Watch. This program reads in 6 CSV files containing data from 2 rounds of data collection, each with 3 sessions per round. It also reads in a JSON file containing session activity data. The program processes the data by combining the data from the CSV files and mapping them to the appropriate activity labels from the JSON file, creating a single activity dataframe. The program includes helper functions for converting timestamps, dividing data into chunks, and creating time deltas. It also includes constants and variables for storing information about the data collection process, such as the number of users and sessions per round, and the columns to be used from the CSV files.

## Data Cleaning
The raw data was stored in CSV files, with each file corresponding to a session. The data was cleaned using the pandas library to extract relevant columns from the CSV files and map activity labels to session logs from a JSON file. This was the resulting file structure:

<img src="https://user-images.githubusercontent.com/108101472/210281998-6386402f-d148-4449-a860-e9dbb2faece8.png" height="400">

## Model Training and Testing
The cleaned activity data was used to train and test the classification model. The model was implemented using CoreML.

## References
Hutcherson, T. (2019, October 9). Activity classification with create ML, COREML3, and skafos: Part 1. Medium. Retrieved January 2, 2023, from https://medium.com/@tyler.hutcherson/activity-classification-with-create-ml-coreml3-and-skafos-part-1-8f130b5701f6 
