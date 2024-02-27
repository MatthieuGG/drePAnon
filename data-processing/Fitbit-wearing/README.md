# Fitbit-wearing

Different methods to estimate from Fitbit minute data if the device was worn or not.
Please consult the [log] at the beggining of the notebook to get information about the features and progress.  

**Warning: the name of columns, file names, key and path may change**

*Step by step description:*
- gather all the physical activity data from fitbit trackers as .csv files in the same folder (see "sample" for an example)
- apply the code provided (**WearingEstimation.ipynb**), which:
    - import all the files as df in Python
    - calculate, for each day, the minute with the minimum calories value
    - define each minute as active if the calorie value is superior to the minimum of the day
    - application of different methods
        - Method 1 = day is considered worn if it contains X active minutes
        - Method 2 = day is considered worn if it contains X hours with X active minutes
        - Method 3 = day is considered worn if it contains X steps
