# NOSQL-Challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom and gives them a food hygiene rating. This study evaluate some of the ratings data in order to help the journalists and food critics decide where to focus future articles, for a food magazine "Eat, Safe, Love".

Deliverable 1: The system imports the data, sets up and updates the uk_food database.

Deliverable 2: The system performs the exploratory analysis queries in the database.

## Part 1: Database and Jupyter Notebook Set Up
1. Import the data provided in the establishments.json file from Terminal.
   Name the database uk_food and the collection establishments. 
   Then import the data from Terminal to a markdown cell in the notebook is provided.
2. Import the libraries needed: PyMongo and Pretty Print (pprint).
3. Create an instance of the Mongo Client.
4. Confirm that the database was created and loaded the data properly with the following parameters:
    Confirm that uk_food is listed in databases in MongoDB.
    List the collection(s) in the database to ensure that establishments is there.
    Find and display one document in the establishments collection using find_one and display with pprint.
5. Assign the establishments collection to a variable to prepare the collection for use.

## Part 2: Part 2: Update the Database
1. Identify a new halal restaurant that just opened in Greenwich in the analysis. 
2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3. Update the new restaurant with the BusinessTypeID found.
4. The magazine is not interested in any establishments in Dover.
   The number of documents contained by the Dover Local Authority was checked and removed.
   The number of documents were re-checked to ensure they were deleted. 
5. Use update_many to convert latitude and longitude to decimal numbers.

## Part 3: Exploratory Analysis
Use the following questions to explore the database, and find the answers, to provide to the magazine editors.
Unless otherwise stated, for each question:
Use count_documents to display the number of documents contained in the result.
Display the first document in the results using pprint.
Convert the result to a Pandas DataFrame, print the number of rows in the DataFrame, and display the first 10 rows.
Which establishments have a hygiene score equal to 20?
Which establishments in London have a RatingValue greater than or equal to 4?
What are the top 5 establishments with a RatingValue of '5', sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.
