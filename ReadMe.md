# Module 12 NoSql Challenge

## Overview

For the Module 12 challenge, we've been asked by the editors of a food magazine, Eat Safe, Love, to evaluate ratings data from the UK Food Standards Agency in order to help their journalists and food critics decide where to focus future articles.

There are two deliverables for this Challenge:
1. Create a Jupyter notebook containing code that imports the data and sets up and updates the uk_food database.
2. Create a Jupyter notebook containing code that performs the exploratory analysis queries in the database.
    
## Files
- 'nosql-challenge'(https://github.com/jackthomas1430/nosql-challenge.git) :The main repo for this challenge. 
    - NoSQL_setup.ipynb: Jupyter notebook containing code that imports the data and sets up and updates the uk_food database.
    - NoSQL_analysis.ipynb: Jupyter notebook containing code that performs the exploratory analysis queries in the database.
    - "Resources": directory containing the ratings data from the establishments.json
    - 'starter_files': contains two jupyter notebooks to use as starter code for the analysis 
    - 'Results': directory containing images of the results 
       
## Instructions

1. Clone the repository to your local device using git clone (https://github.com/jackthomas1430/nosql-challenge.git)
2. Activate virtual enviroment using the following command in your terminal: 'conda activate dev' 
3. Ensure MongoDB is running locally
4. Import data: to import the data provided in the establishments.json file navigate to the directory containing the Resources folder on your terminal and run the following command:mongoimport --db uk_food --collection establishments --drop --file establishments.json --jsonArray
5. Open the Jupyter Notebook named NoSQL_setup.ipynb and run to import the data and set up and update the uk_food database
6. Open the Jupyter Notebook named NoSQL_analysis.ipynb and run to execute the exploratory analysis queries in the database

## Results/Analysis: 
1. Which establishments have a hygiene score equal to 20?
There are 41 establishments with a hygiene score equal to 20 
![question_1](nosql-challenge/Results/question_1.png)
2. Which establishments in London have a RatingValue greater than or equal to 4?
There are 33 establishments in London with a RatingValue greater than or equal to 4
![question_2](nosql-challenge/Results/question_2.png)
3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
![top_5](nosql-challenge/Results/question_3.png)
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
![hs_o](nosql-challenge/Results/question_4.png)

     
## Acknowledgements

Xpert Learning Assistant was used to answer detailed questions, and assist in debugging.For more information about the Xpert Learning Assistant, visit [EdX Xpert Learning Assistant](https://www.edx.org/). 
    
## References
- PyMongo Documentation[https://www.mongodb.com/docs/manual/]
