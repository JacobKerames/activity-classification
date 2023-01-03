# Activity Classification Model

<img src="https://user-images.githubusercontent.com/108101472/209432584-311c4ce0-61c6-4bef-be80-5ddf492a381c.png" width="1000">

This project involves processing and analyzing data from the accelerometer and gyroscope sensors of an Apple Watch to classify various activities. The raw motion data was obtained from an Apple Watch.

Purpose
The purpose of this project is to develop a model that can classify various activities based on data from the accelerometer and gyroscope sensors of an Apple Watch. This can potentially have a variety of applications, such as tracking physical activity or monitoring the movements of individuals for safety purposes.

Code
The code for processing and analyzing the data is written in Python and makes use of the pandas library. The code includes several helper functions for handling timestamps and splitting lists into smaller chunks. To run the code, you will need to have the following dependencies installed:

pandas
Instructions for running the code and any necessary input/output files are included in the comments of the code itself. The code performs the following tasks:

Import necessary libraries and constants
Read in .csv files containing the raw sensor data from multiple sessions
Load a .json file containing activity labels for each session
Process and clean the sensor data, including converting timestamps to a consistent format and selecting relevant columns
Create a dataframe of activity labels and sensor data for each session
Concatenate the dataframes for each session into a single dataframe
Save the resulting dataframe to a .csv file
The resulting dataframe is saved to a .csv file in the output directory. The file is organized into two sets: a training set and a testing set. The training set includes data from both rounds of data collection, while the testing set includes data from only one round.

Data
The raw data from the accelerometer and gyroscope sensors is included in the data directory. The data is provided in .csv format and is organized by round of data collection (two rounds in total) and session within each round. Each session includes data from one user.

<img src="https://user-images.githubusercontent.com/108101472/210281998-6386402f-d148-4449-a860-e9dbb2faece8.png" height="400">

## Model Training and Testing
The cleaned activity data was used to train and test the classification model. The model was implemented using CoreML.

## References
Hutcherson, T. (2019, October 9). Activity classification with create ML, COREML3, and skafos: Part 1. Medium. Retrieved January 2, 2023, from https://medium.com/@tyler.hutcherson/activity-classification-with-create-ml-coreml3-and-skafos-part-1-8f130b5701f6 
