# ActivityClassificationModel

This repository includes data, code, and information outlining the procurement of testing and training data for an activity classification machine learning model in Create ML. The model will provide detection of an activity with either hand, or a lack thereof in watchOS application.

# What I Learned

* Raw accelerometer and gyroscope data was collected from an Apple Watch in the form of .csv files.
* A .json activity label log was created to specify the rounds, sessions and activities of the raw data samples with time stamps.
* Python was used in Google Colaboratory with the pandas library to condense all raw data into one file and add activity and session labels to over 50,000 samples.
* Python was then used with the Turi Create library to create multiple .csv files. Each file includes accelerometer and gyrometer data of an activity and were used to train and test the activity classification machine learning model in Create ML.

Portions of this work has been adapted from:
https://github.com/skafos/ActivityClassifier
