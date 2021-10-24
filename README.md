# Movies-ETL -Amazing Prime



## Project Description and Purpose
_______________________________________

Amazing Prime is a online retailer that streams tv shows and movies. After our initial project, Amazing Prime would like us to refactor our code to manage the data sources and keep it updated daily. We are continuing work with Britta and will be continuing our work with data from Wikipedia and Kaggle. The code will automate the process of taking in the new data, ceaning the data and restructuring it to be loaded into our existing tables. Amazing Prime is preparing for a hackathon, which is an event where teams of analysts work collectively to solve a problem and use the clean data we have put together. The purpose of our ETL process is to, extract the Wikipedia and Kaggle data from their source and transform the datasets. We wil combine data, remove unwanted columns, decrease the data by dropping the data sets that have no values. After cleaning up the dataset we will be joining them together, and load the cleaned dataset into a SQL database.


## Prepering the Data for the Hackathon
____________________________________________________________
We start by creating a function to load in the Wikipedia data, Kaggle Metadata, and the MovieLens Rating Data. We create three data frames from each data source to be cleaned.


<img width="499" alt="Function to read the three filesPNG" src="https://user-images.githubusercontent.com/88467263/138615486-46dc4e12-d958-4850-b9b4-269bb4a8cd54.PNG">



### Extract and Transform the Wikipedia Data and merge it with the Kaggle metadata.
____________________________________________________________________

We refactor the code from our previous project using the clean movie function. Next we read in the three data files and using list comprehension we filter out TV shows from the Wiki Movies file. We used try and except function with regular expressions to catch errors while working with the IMDB IDs. We used list comprehension to remove duplicates and null values and create our cleaned up dataframe from list. We consolidated the data columns from almost 200 to 21 useful columns to be loaded into our SWL Database. We formatted our release dates, budgets and various column data before loading into our SQL database.

<img width="433" alt="ETL_clean_wiki_movies" src="https://user-images.githubusercontent.com/88467263/138615492-cab7e44e-e6da-4608-b7f9-a53ecce81b92.PNG">



In our final steps we loaded our DataFrames into a SQL Database. We were able to scrape in data and develop a user friendly analysis for the hackathon. Amazing Prime will be able to put on a successful event and Britta will be proud of our hard work. In the end we developed efficient code that will be useful in keeping up with changing data. The steps taken to clean the data will be useful for many futre events.

### Loading Data into SQL Database

<img width="737" alt="movies_query" src="https://user-images.githubusercontent.com/88467263/138615500-188532ff-7a74-48b6-af9e-336b7967c981.PNG">

<img width="298" alt="ratings_query" src="https://user-images.githubusercontent.com/88467263/138615503-dc5ebf31-13e5-4cac-a7fa-aaa2b4dc6ef4.PNG">
