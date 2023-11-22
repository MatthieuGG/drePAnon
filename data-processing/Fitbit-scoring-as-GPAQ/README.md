# How to obtain MET-min/week using Fitbit data as GPAQ scores  

Fitbit PA trackers can provide you steps, kcal, MET and intensity of PA per minute. Based on the GPAQ calculation, you can obtain the number of minutes per week spend practicing moderate (MPA), vigorous (VPA), or no physical activity; then translate it into MET-min/week.  
It is important to note than the GPAQ calculation is particular because 1/ it doesnt take light physical activity into consideration, 2/ it only considers bouts of 10 minutes of phycisal activity, 3/ it considers moderate physical activity from 4 to 8 MET, and vigorous above 8.

To do so, you need to:  
- get all the .csv files with per-minute PA data and put them all in the same folder (see "sample")
- use the code provided (**Scoring Fitbit as GPAQ.ipynb**) on your transposed .csv files to obtain the energy expenditure over a week. You have to precise the path of the folder where all the .csv are, and the path where you want to save the result
