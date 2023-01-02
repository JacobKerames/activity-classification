# Motion Data Collection for Activity Classification

<img src="https://user-images.githubusercontent.com/108101472/209432584-311c4ce0-61c6-4bef-be80-5ddf492a381c.png" width="1000">

This program is used to parse and combine data from multiple sessions of data collection for a research project. The data consists of sensor readings from participants' watches and activity labels recorded during the sessions.

# How the Program Works

The program begins by importing some constants and libraries, including json, datetime, csv, and pandas. Then, it loads in six data files containing sensor readings from participants' watches, as well as a sessions_log.json file containing activity labels recorded during the sessions.

Next, the program defines some constants, including rounds, users_per_round, and sessions_per_round, and some helper functions, including convert_timestamp, chunks, and make_delta. These constants and functions will be used later in the program to manipulate the data.

The program then iterates through the rounds of data collection and the sessions within each round. For each session, it loads the activity labels and sensor data for each participant, combines them into a single dataframe, and appends the dataframe to a list of dataframes for all sessions.

Finally, the program concatenates the list of dataframes into a single dataframe containing all the data from all sessions, and writes the dataframe to a new CSV file called combined_data.csv.

# Running the Program

To run the program, make sure you have the necessary libraries installed and the required data files in the same directory as the program file. Then, simply run the program using your preferred method (e.g. python program.py). The program will output progress messages as it parses and combines the data, and will create a new combined_data.csv file when it is finished.

# Data Files

The program expects the following data files to be present in the same directory:

    watch_round1_session1.csv
    watch_round1_session2.csv
    watch_round1_session3.csv
    watch_round2_session1.csv
    watch_round2_session2.csv
    watch_round2_session3.csv
    sessions_log.json

Each of these files contains data from a specific session of data collection. The watch files contain sensor readings from participants' watches, while the sessions_log.json file contains activity labels recorded during the sessions.

# Output File

The program will create a new combined_data.csv file in the same directory as the program file. This file will contain all the data from all sessions, with the activity labels and sensor readings for each participant combined into a single row.
