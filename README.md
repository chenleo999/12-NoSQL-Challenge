# 12-NoSQL-Challenge

completed by Li Chen  2/27/2024

Part 1 NoSQL_setup_starter.ipynb

steps
1- import josn file from terminal, copy/paste mongoimport command into markdown cell in Jupyter Notebook file
2- create mongo client instance, assign database/collection to variables
3- confirm successful import, check 1 document
4- insert 1 new document with given data, confirm insert success 
5- query collection for new record's Business Type, identify Business Type ID in database
6- update the newly inserted record with the identified Business Type ID, confirm update success 
7- count and remove documents with Local Authority Name = Dover, confirm delete success
8- change data type: lat/lon to double, set non-numeric ratings to None, then change rating data type to integer, confirm update success


Part 2 NoSQL_analysis_starter.ipynb

steps:

Question 1
query in documents for Hygiene score = 20
count records, pprint 1st
conver results to Pandas DataFrame and display head 10

Question 2
query in documents for Local Authority Name like '%London%' and Rating >= 4
count records, pprint 1st
conver results to Pandas DataFrame and display head 10

Question 3
query in documents for top 5 that Rating=5 and close to Penang Flavour (with 0.01 degree of lat/lon), sort by Hygiene score in ascending order
pprint all 5 
conver results to Pandas DataFrame and display all rows

Question 4
build pipeline as:
    match in documents for Hygiene score = 0
    group matched documents by Local Authority Name, get counts in each group
    sort results by counts in descending order

aggregate documents with the pipeline 
pprint first 10 
conver results to Pandas DataFrame and display head 10




