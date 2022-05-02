# SURFS_UP
## Overview of the analysis

The purpose of this analysis is to perform an analysis on the trends in temperature in Oahu, Hawaii being that we are trying to analyze the profitability of surf-ice cream shop during the months of June and December.
We chose those months as a sample so that our client can make a more informed decision.

## Results 
The following are the statistical results for the months of June and December

![image](https://user-images.githubusercontent.com/99924850/166172346-bd19bcdd-db3a-4f90-9f01-478bbcbe4242.png)

![image](https://user-images.githubusercontent.com/99924850/166172372-60f4e4d2-1e5d-4452-99b7-81ea0414b9ac.png)

Based on those results we can conclude the following
-the average temperature in December is 3.9 degrees lower than the one in June
- the lowest temperature in December is 8 degrees colder than the lowest temperature in June
- the highest temperature in June and December seem to be almost the same as there is only a 2 degree difference between the highest temperature in December and the highest temperature in June 

## Summary

Based on the analysis above we can see that our customer is to excpect more customers in June than December as the temperature are clearly at the highest and who does not want to surf and sweet ice cream when its hot.

We can however perform a new querry and analysis based on precipitation as we all know this can also impact a business of surf and ice-cream during the months of June and December for a more detailed analysis and to avoid surprises when the shop is already running
The following querries can be used to perform said analysis 
***June Query***
```
session.query(Measurement.date, Measurement.prcp).\
filter(extract('month', Measurement.date) == 6).all()
```
To view the statistics results [click here]https://github.com/fofoMichelle/surfs_up/blob/main/Resources/june%20precip%20stats.png

**December query***

```
session.query(Measurement.date, Measurement.prcp).\
filter(extract('month', Measurement.date) == 12).all()
```

To view the statistics results of December [click here]https://github.com/fofoMichelle/surfs_up/blob/main/Resources/december%20precip%20stats%20.png

We can do another analysis based on the precipitations of June and December. 
For more questions and inquiries please contact me via [Linkedin]

