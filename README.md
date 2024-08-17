# Movie Recommender System

## Overview
This Movie Recommender System is a content-based filtering application developed using Python. It utilizes movie metadata such as genre, cast, crew, and keywords to recommend movies similar to the ones the user likes. The system calculates the similarity between movies using techniques like CountVectorizer and cosine similarity.

## Features
Content-Based Recommendations: Suggests movies similar to a given movie based on their content (e.g., genre, cast, crew).
Simple Interface: Users can input a movie title, and the system will return a list of recommended movies.

## Dataset
Movies.csv: Contains metadata for each movie such as title, genres, keywords, cast, and crew.
Credits.csv: Contains additional details about the cast and crew for each movie.

## How to Use
### Load the Data:
The system begins by loading the movie and credit datasets using pandas.

### Data Preprocessing:
The two datasets (Movies.csv and Credits.csv) are merged based on the movie title.
Unnecessary columns are dropped to keep only relevant information.

### Feature Extraction:
Text data such as genres, keywords, cast, and crew are processed using CountVectorizer to convert text into a matrix of token counts.

### Calculate Similarity:
The similarity between movies is computed using the cosine similarity metric, which is particularly effective in handling high-dimensional data.

### Movie Recommendation:
The system provides a list of movies similar to the movie input by the user.
Recommendations are made based on the top N most similar movies.

## Running the System
### Launch Jupyter Notebook:
Open the notebook Movie Recommender System.ipynb in Jupyter Notebook or JupyterLab.

### Run the Cells:
Execute the cells in the notebook sequentially to load data, preprocess it, compute similarities, and finally generate movie recommendations.

### Input Movie Title:
Modify the relevant cell to input your desired movie title and run it to get a list of recommended movies.

## Example
If you input the movie title "Avatar", the system will return a list of movies similar to "Avatar" based on the calculated content similarity.
