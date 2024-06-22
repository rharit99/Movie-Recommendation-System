# 🎬🍿 Movie-Recommendation-System

# Movie Recommendation System

## Overview

This project focuses on building a content-based movie recommendation system using a dataset of movies. It processes metadata and employs machine learning techniques to suggest movies similar to a user's interests.

## Data Preprocessing

- Loaded movie data from `credits.csv` and `movies.csv`.
- Merged both datasets on the movie title for a comprehensive view.
- Selected relevant columns and dropped missing values.
- Deduplicated the dataset to maintain data integrity.
- 
## Feature Engineering

- Converted genre, keyword, cast, and crew details from JSON to lists.
- Extracted the director's name from the crew.
- Processed the overview and other text features to prepare for vectorization.

## Text Processing

- Implemented custom functions to transform and clean text data.
- Applied the `ast` module to parse stringified lists of dictionaries.
- Utilized `nltk` and `PorterStemmer` for stemming text data, reducing words to their root form.

\
## Vectorization

- Utilized `CountVectorizer` to convert the 'tags' feature into numerical data, allowing for the application of machine learning algorithms.
- The vectorization process created a vocabulary from the 'tags' text and transformed the dataset into a sparse matrix based on word frequencies.

## Similarity Calculation

- Calculated cosine similarity among movies based on their tag vectors, providing a measure of content similarity.

## Recommendation Function

- Created a function `recommend` that takes a movie title as input and outputs a list of similar movies based on content similarity.

## Usage

<img width="559" alt="Screenshot 2024-04-07 at 12 10 47 AM" src="https://github.com/rharit99/Movie-Recommendation-System/assets/159074503/f23f37f1-337d-4847-aee5-3c6646dd2e76">

