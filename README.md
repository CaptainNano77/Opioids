# Opioids
This repository (My Current Project!) contains analysis of opioid prescribers in the USA.
My goal is to predict which medical professionals would be considered "opioid prescriber's" based on features such as gender, degree, and a list of different prescribed pharmaceuticals. 

I hope to then merge these with other analysis of an overdose database...

There are several notebooks available:
1) Opioids.ipynb: This was the first notebook. It has all of the EDA and initial models. It has a lot of regex work that I did on the degree feature as well.

2) Opioids_noDrugFeatures.ipynb: This is the 2nd notebook. I did the EDA and machine learning on ONLY the features that were not drugs. There seemed to be 2 questions here...a) did non-drug features such as gender and degree have predictive power and b) did the drug columns have predictive power.

3) Opioids_DrugOnlyFeatures.ipynb: This is the 3rd notebook. I did the EDA and ML on ONLY the drug columns. 

4) Opioids_Overall.ipynb: This was the 4th notebook and has the top non-drug and drug features (from notebooks #2-3).

Turned out that only the drug features were needed. A random forest model was chosen to be best with drug only features.

DATA:
1) prescriber-info.csv: Original prescriber data 
2) prescriber_clean.csv: The cleaned prescriber data. Has the degrees formatted and the such (the work I did in the 1st notebook (Opioids.ipynb)
3) prescriber_top100drug.csv: The prescriber data that is cleaned and only contains the top 100 drug features.
4) opioids.csv: List of the drugs and names
5) overdoses.csv: The data that I am now hoping to merge with this "prescriber" work to see if there are overdose correlations, etc.
