# NoSQL Challenge

## Purpose

The UK Food Standards Agency evalutes various establishments across United Kingdom, and gives thema food hygiene rating. My function is evaluate some of the ratings data.

## Solution Files

I received two files for started code:

- NoSQL_setup_starter.ipynb
- NoSQL_analysis_starter.ipynb

### Steps and screenshots of the results for the file NoSQL_setup_starter.ipynb

- Import the data provided establishments.json using the terminal with the code:
  - mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

- Import the libraries,

  ![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/c8f51abe-b544-4d9a-bc3c-93e98dc4252a)

- Create an instance of the Mongo Client,
- Create database, list the collections in the database.
- Display one document:

![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/569d62b3-4f0d-4d32-bf0b-3c325e687696)

- Add a new restaurant:

![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/b3a387c4-a769-4f14-aa4b-bf636d97ab42)

- Find the BussinessTypeID for "Restaurant/Cafe/Canteen" and return the only the required fields.
- Update the new restaurant BussinessTypeID.
- Remove any establishments within the Dover localtion Local Authority from the data base.
- Convert latitude and longitude to decimal numbers.
- Convert RatingValue to integer numbers

### Steps and screenshots of the results for the file NoSQL_analysis_starter.ipynb

Answer the questions for analyse the data:

1. Which establishments have a hygiene score equal to 20?

![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/56c74d40-20b8-44f8-8aa5-40fd69b2b134)

2. Which establishments in London have a RatingValue greater than or equal to 4?

![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/e654854b-6347-490b-9a7a-110346c5d2b6)

3. What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0? Sort the results from highest to lowest, and print out the top ten local authority areas.

![image](https://github.com/KamillaToberia/nosql-challenge/assets/145527812/c64bd41e-a67b-4448-ab77-cc3c9a65d413)

## References

UK Food Standards Agency (2022). UK food hygiene rating data API. https://ratings.food.gov.uk/open-data/en-GB. Contains public sector information licensed under the Open Government Licence v3.0
Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
