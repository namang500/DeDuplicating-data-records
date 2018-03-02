# DeDuplicating-data-records
finding duplicate entries


This project is about de-duplicating entries in data entries.
The dataset consists of 5000 entries with 1000 entries duplicated , the duplicated entries varies from [none - 5] entries 
per data entry(whiich consists of names , dob , gender)

First of all , the data entry is cleaned to extract the important features which are required to find the duplicacies .
the names are cleaned which consists of ["Mr." , "Mrs." , "Jr." , "Sr." ,etc. ] vain data.
date of birth is also formated form ["/" to ""]

then the dataframe is sub-divided using Block Indexing where the entries with more related and similar entries are clubbed together 
this helps in reducing the no. of comparisions , since the dataset can consist of millions of entries and comparing those entries with
each other can be time consuming , so , its better to sub divide the data so that it can reduce comparisons.

then the comparision are made so as to compare those entries which lie in same block indexes so , as to find similar entries , may contains 
entries with just one similar column or multiple similar columns

the data similarity matrix is then printed so , as to analyse the mean , standard deviation and other important features

and finally , the duplicated values are printed which contains all similar column values
