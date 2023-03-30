# nosql-challenge
Module 12 Challenge

Included are the two notebooks for the nosql challenge.  The command line to import the data and create the 'establishments' collection is:
mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json  An alternate way is to use the import function of MongoDB Compass.

The starter code assigns variable names to the database and collection, and verifies the database.  I then added a restaurant to the database and updated the Business Type ID and Business Type fields.  I then removed restaurants in Dover and converted longitude and latitude to decimal format.

In the analysis code, I identified restaurants with a hygiene score of 20 and created a dataframe.  I then queried for restaurants in London with a Rating Value greater than or equal to 4 and converted those results to a dataframe.  I then looked for restaurants near the new restaurant we created in the previous notebook with a Rating Value of 5.  Those results were sorted by lowest hygiene score and converted to a dataframe.  Finally, I looked for establishments with a hygiene score of 0 and grouped those to get a count for each area.

Using Pandas and dataframes gave this challenge a familiar feel, even though we were using new tools with MongoDB.  It's helpful to see how all these programs/languages can be used together.
