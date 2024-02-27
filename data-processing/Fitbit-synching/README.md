# Fitbit-synching

This methods permits to obtain information about data lost and synchronisation, based on the comparison between minute and daiy resolution data.
  
Whith a 5-7 days memory capacity, the Fitbit smartwatch can retain minute resolution data for 5-7 days between 2 synchs. After this period of time, the watch stops reccording minute data, and only reccords on a daily basis.  

As we have access to minute and daily Fitbit data, we just have to compare the minutes data resampled by day to the daily data. If we observe a difference on day n, we can tell that there was no synchronisation 5 days after (n+4).
With this code, all you have to do is:
- gather all your Fitbit data (minute and daily) as .csv files according to the tree structure shown (sample/min & sample/daily)
- apply the code provided (**SynchingEstimation.ipynb**)
- be carefull to the name of columns in the results
- please note that the information (synch) is a booleen type
- also, please note that the memory capacity may vary from watches model. Please modify the memory_capacity
