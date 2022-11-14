# ActivityClassificationModel

This GitHub repository includes data, code, and information outlining the procurement of training and testing data for activity classification in Create ML. The process includes raw motion data collection, labeling, and cleaning. The trained model will provide detection of an activity with either hand, or a lack thereof, in a watchOS application.

# Steps

* Collect raw accelerometer and gyroscope data from an Apple Watch, in the desired frequency, and output to .csv files.
* Create a .json activity label log to specify the rounds, sessions, and activities of the raw motion data samples, using time stamps.
* Open Python in a console and use the pandas library to compile all raw motion data into one file and specify the session and activity of each sample.
* In the Python console, use the Turi Create library to create multiple .csv files containing samples of a specific activity. These files will then be used to train and test the machine learning model.

Portions of this work has been adapted from:
https://github.com/skafos/ActivityClassifier
