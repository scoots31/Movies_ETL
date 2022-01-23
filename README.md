# Extract, Load, Transform Movies_ETL
Amazing Prime, the World's largest online retailer sponsored a hackathon asking participants to predict popular movies. Their goal was to determine which low budget movies being released would become popular so they could buy the streaming rights at a bargain. Brita is creating data sets for the hackathon and has the following information:
	
  •	Wikipedia Movies released from 1990
  
  •	Ratings data from movielens a site run by the GroupLens research team which has over 20 million moving ratings

In order to make information available for the hackathon Brita needs to extract the movie data, transform it, and load it into a SQL database for access by the participants.

Below is that ETL process.

## Write an ETL function to read three data files
The function takes the Wikipedia JSON, the Kaggle metadata and MovieLens csv files and creates three separate DataFrames.

## Extract and Transform the Wikipedia data
We filtered out the TV shows, consolidated the redundant data, removed the duplicates and formatted the Wikipedia data.

## Extract and Transform the Kaggle and rating data
Again, we consolidated the redundant data, removed the duplicates, formatted and grouped the data.
The Kaggle and rating data were then merged with the Wikipedia movies DataFrame.

## Load the data to a PostgreSQL Movie Database
