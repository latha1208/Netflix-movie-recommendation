# Netflix-style Movie Recommendation System

## Project Overview

A simple but powerful movie recommendation system built on the MovieLens dataset (~100k ratings).  
This system suggests movies similar to a given movie using **Pandas** and **Cosine Similarity**.

## Dataset

- Source: [MovieLens Latest Small Dataset](https://grouplens.org/datasets/movielens/)
- Files: `movies.csv`, `ratings.csv`

## Key Technologies

- Python
- Pandas
- Scikit-learn (Cosine Similarity)
- Google Colab

## How It Works

1. Load user ratings and movie metadata.
2. Create a user-movie pivot matrix.
3. Fill missing ratings with 0.
4. Transpose the matrix for movie similarity.
5. Calculate cosine similarity between movies.
6. Recommend top N similar movies.

## How to Run

1. Open `Movie_Recommendation.ipynb` in Google Colab.
2. Upload `movies.csv` and `ratings.csv`.
3. Run all the cells.
4. Use `find_movie_id('Movie Name')` to find movieId.
5. Use `recommend_movies(movieId, N)` to get recommendations.

## Example

```python
find_movie_id('Toy Story')
recommend_movies(1, 5)
