This folder contains the ground truth data from the task distributions forms set to the volunteers.
These files are created from the /data_preprocessing_scripts/convert_task_distribution.py script with the following task distribution files:

- Task distribution20200320.csv
- Task distribution20200324.csv
- Task distribution20200325.csv


**requests_train.csv** - Contains the requests that appear in the task distribution forms sent to the volunteers. 


**responses_train.csv** - Contains the rating of the volunteers for each request/task. The column 'volunteer' matches the column 'volunteer' in the ../volunteers.csv file. The column 'request' matches the column with the same name in the requests_train.csv file of this folder. 

The 'request' column in both files matches but we do not have yet a match with the to-be-constructed requests.csv file (coming from the new ticketing system). 