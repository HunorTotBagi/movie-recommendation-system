# Movie Recommendation System

This movie recommendation algorithm uses regular expressions to clean movie titles, creating a TFIDF matrix. It calculates similarity between entered and existing movies using cosine similarity and incorporates user preferences and ratings data to recommend movies liked by similar users. The algorithm assigns recommendation scores based on user percentages.

## Prerequisites

- `Python 3.x`

Before running the code, ensure that you have the following libraries installed:

- `scikit-learn`
- `pandas`
- `numpy`
- `IPython`
- `ipywidgets`

You can install the required dependencies using pip:

```
pip install scikit-learn pandas numpy IPython ipywidgets

```

## Data

The code uses two datasets for movie recommendations:

- Movies dataset: This dataset contains information about movies such as movieId, title, and genres. The dataset is available in the file `movies.csv`. You can download the dataset from the following link: [MovieLens Dataset](https://files.grouplens.org/dataset/movielens/ml-25m.zip)
- Ratings dataset: This dataset contains movie ratings given by users. The dataset is available in the file `ratings.csv`

## Code

The code provided implements a movie recommendation system using TF-IDF (Term Frequency-Inverse Document Frequency) and cosine similarity. It performs the following steps:

- Cleans the movie titles using regular expressions to remove any non-alphanumeric characters
- Creates a TF-IDF matrix using the cleaned movie titles
- Defines a search function that computes the similarity between a given movie title and all movies in the dataset using cosine similarity
- Finds users who have rated and liked a specific movie
- Retrieves other movies liked by those users
- Calculates the recommendation score for each movie based on user similarity and movie ratings
- Generates a list of recommended movies sorted by the recommendation score

## Output

The code outputs the following information:

- Similar movies based on the search query provided
- Users who have liked the searched movie and other movies they have rated highly
- Recommended movies based on user similarity and movie ratings, sorted by recommendation score

The output includes movie details such as movieId, title, genres, and clean title.
