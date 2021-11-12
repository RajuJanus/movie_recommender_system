# Movie_recommender_system
In this file two movie recommendation systems are developed based on datasets provided by MovieLense.
One is popularity based. The second one is based on similarity among the user tastes, e.g. the users who likes similiar movies.

# Technologies
pandas 1.3.3

matplotlib 3.4.2

seaborn 0.11.2

sklearn 0.24.2

numpy 1.21.4

# Steps
A. Popularity based recommendation
we group the ratings by movie Id and sort them in descending order to get top 5 popular movies e.g. the movies most of the users rated.
B. Similarity based reccomendation: cosine similarity

1. Building a Recommender function from scratch (Iteration 1): imputing NaN's with 0, Cosine similarity matrix
2. Make a train-test split of the data and do the same (Iteration 2)

# Data
This dataset describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 100836 ratings and 3683 tag applications across 9742 movies. These data were created by 610 users between March 29, 1996 and September 24, 2018. This dataset was generated on September 26, 2018.

Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

The data are contained in the files `links.csv`, `movies.csv`, `ratings.csv` and `tags.csv`. More details about the contents and use of all these files follows.

This is a *development* dataset. As such, it may change over time and is not an appropriate dataset for shared research results. See available *benchmark* datasets if that is your intent.

This and other GroupLens data sets are publicly available for download at <http://grouplens.org/datasets/>.
