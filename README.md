## Gun-Related Crime Vs. Gun Laws

#### Final Project for Code Louisville May 2018 Python Course

This is a project using Python in a Jupyter Notebook to answer a question 
about a dataset using SQL queries and a database. The question I am attempting
to answer relates to gun-related crime in the United States.  The question is:  

___

> **Is there a relationship between the amount of gun-related crime and the strictness of laws concerning guns (measuring for each U.S. state)?  In other words, how effective are gun laws?**

___

To accomplish this, I gathered the needed data from each database (incidents from `Gun_Violence_Data` and laws from `State_Firearm_Law_Database`) and separated them out into tables by state (one for laws, one for incidents).  Within `State_Firearm_Law_Database`, each law is described as restrictive, permissive, or neither. To determine a state's strictness on firearms, I scored them by totaling the laws labeled 'permissive' in the database and subtracting them from those labeled 'restrictive'. Then, to answer the question, I took the results of these equations and plotted them against the average number of gun-related incidents by the years sampled. Those years were 2014-2017 and were based on the information available in the datasets.   

The dataset also included 2013 and 2018, but the information for those years was incomplete, so it was edited out in order to abbreviate what was rather bulky dataset of ~200,000 entries.

---

#### Files used:

`csv_files/Gun_Violence_Data.csv`  
downloaded from *[here](https://www.kaggle.com/jameslko/gun-violence-data)*

`csv_files/State_Firearm_Law_Database.csv`  
downloaded from *[here](https://www.rand.org/pubs/tools/TL283.html)* (The base file is in .xlsx format with formatting. To view the cleaned-up version, follow this *[link to the Google Sheets Doc](https://docs.google.com/spreadsheets/d/1hGbucoI2RCAdkdSI7C4GYLoGaSansGANfqxXobpIrog/edit?usp=sharing)*)  

---

***To view this project, you will need the following installed on your computer:***  

* Jupyter Notebooks (as part of Anaconda Navigator or otherwise)
* DB Browser for SQLite