# nosql-challenge
"The UK Food Standards Agency evaluates various establishments across the United Kingdom, 
and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, 
Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists 
and food critics decide where to focus future articles."

### Part 1:

Imported data from JSON file. 
Imported the PyMongo & Pretty Print libraries.
Created instance of Mongo Client and confirmed the database was created and loaded properly.
Assign the establishments collection to a variable.
Prepare the collection for use.

### Part 2:

Update the Database
Add information for a new hala restaurant in Greenwich.

Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.

Update the new restaurant with the BusinessTypeID you found.

The magazine is not interested in any establishments in Dover, 
so check how many documents contain the Dover Local 
Authority. 
Then, remove any establishments within the Dover Local Authority from the database, 
and check the number of documents to ensure they were deleted.

Some of the number values are stored as strings, when they should be stored as numbers.

Use update_many to convert latitude and longitude to decimal numbers.

Use update_many to convert RatingValue to integer numbers.

### Part 3: 

Exploratory Analysis

Eat Safe, Love has specific questions they want you to answer, which will help them find the locations they wish to visit and avoid.

Use NoSQL_analysis_starter.ipynb for this section of the challenge.

#### Which establishments have a hygiene score equal to 20?

There are 41 establisments with a hygiene score equal to 20.

Which establishments in London have a RatingValue greater than or equal to 4?

There are 87 establisments with a RatingValue greater than or equal to 4.

What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

Howe and Co Fish and Chips - Van 17
Lumbini Grocery Ltd T/A Al-Iman
Atlantic Fish Bar
Iceland
Volunteer

How many establishments in each Local Authority area have a hygiene score of 0? 
Here are the first 10 Local Authority areas in our results with their count of how many establishments have a hygiene score of 0:
