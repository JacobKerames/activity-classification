# Activity Classification Model

<img src="https://user-images.githubusercontent.com/108101472/209432584-311c4ce0-61c6-4bef-be80-5ddf492a381c.png" width="1000">

This project involves the creation of an activity classification model that detects hand movement or lack thereof using raw motion data from an Apple Watch. The data was collected in two rounds, with each round containing data from one user across three sessions.

## Data Cleaning
The raw data was stored in CSV files, with each file corresponding to a session. The data was cleaned using the pandas library to extract relevant columns from the CSV files and map activity labels to session logs from a JSON file. This was the resulting file structure:

<img src="https://user-images.githubusercontent.com/108101472/210281998-6386402f-d148-4449-a860-e9dbb2faece8.png" height="400">

## Model Training and Testing
The cleaned activity data was used to train and test the classification model. The model was implemented using CoreML.

## References
Hutcherson, T. (2019, October 9). Activity classification with create ML, COREML3, and skafos: Part 1. Medium. Retrieved January 2, 2023, from https://medium.com/@tyler.hutcherson/activity-classification-with-create-ml-coreml3-and-skafos-part-1-8f130b5701f6 
