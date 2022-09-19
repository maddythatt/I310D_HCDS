# I310D_HCDS
# Licensing
I retrieved the raw data from ProPublica Data Store, the name of the data was "Clinical Trials: Participant Demographic Data" and the source for these findings was the U.S. Food and Drug Administration, Drug Trial Snapshots. Due to the data terms of use via ProPublica Data Store - 
(https://www.propublica.org/datastore/terms)
I'm unable to upload or republish the raw data in it's entirety, so I have linked the web page of where I accessed the free download - 
(https://www.propublica.org/datastore/dataset/cancer-clinical-trials-demographics-data).

# Project Summary / Goal of Project
The data was orignally collected to demographically breakdown patients that participated in several clinical trials for various FDA-approved drugs, this information was accrued during the window of January 2015 to June 2018. The columns or attributes of the dataset are broken down by drug name: **Brand Name**, drug treatment description: **Indication**, racial identity: **White**, **Black or African American**, **Asian**, **Hispanic or Latino (2017 only)**, **All Other (Aggregrated) - American Indian/Alaska Native, Native Hawaiian, or Other Pacific Islander**, gender: **Women**, age: **≥65**, **≥75**, **≥80**, **U.S. Only (2017 only)**, **Year**, and **Notes**. Using this dataset, I primarily focused on patients who were Asian and specifically the types of drugs that only held 1% of representation. My goal for solely highlighting Asian representation in these clinical trials, is to provide a dataset and pathway for a future study to be conducted in better understanding what health problems are of more concern within the Asian community. 

# Issues / Biases
Within the description of the raw data from ProPublica, it was established that the "Hispanic or Latino" category was not included in the yearly summary reports for 2015 to 2016, therefore information gathered for that race in particular is not included within my final processed dataset. It was also made known that although the FDA typically provides demographic breakdowns by drug with more detailed information, raw numbers for patients, and occasionally disaggregated "Other" categories they did not include that information in the ProPublica published data and therefore it is not included in my final processed dataset as well.

# Data Dictionary
*Columns with two data types `str` and `float` were converted during data processing* 
**Brand Name** (class `str`): Name of drug
**Indication** (class `str`): Description of drug treatment 
**Women** (class `str`)/(class `float`): Patients of female gender identity 
**White** (class `str`)/(class `float`): Patients of White/Caucasian racial idenity
**Black or African American** (class `str`)/(class `float`): Patients of Black/African American racial identity
**Asian** (class `str`)/(class `float`): Patients of Asian racial idenity
**Hispanic or Latino** (class `float`): NaN 
**All Other (Aggregated)** (class `str`)/(class `float`): Patients of American Indian/Alaska Native, Native Hawaiian, or Other Pacific Islander racial identity
**U.S. Only (2017 Only)** (class `float`): NaN
**Age 65 and Older** (class `str`)/(class `float`): Patients age 65 and older
**Age 75 and Older** (class `str`)/(class `float`): Patients age 75 and older
**Age 80 and Older** (class `str`)/(class `float`): Patients age 80 and older
**Year** (class `numpy.int64`):NaN
**Notes** (class `float`): NaN
