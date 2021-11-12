# Movie_recommender_system
In this file, two movie recommendation systems are developed based on datasets provided by MovieLens.
The first one is popularity based and the second one is based on similarity among the user tastes, e.g. the users who like similiar movies. 
The similarity is deduced by calculating cosine similarity matrix.
At the end, error analysis, such as, absolute error/mean square error/root mean square error calculation are also conducted by splitting the dataset between train and test using scikit metrics. The result is visualized by using seaborn library.

# Technologies
pandas 1.3.3

matplotlib 3.4.2

seaborn 0.11.2

sklearn 0.24.2

numpy 1.21.4

# Steps
A. Popularity based recommendation

  we group the ratings by movie Id and sort them in descending order to get top 10 popular movies e.g. the movies most of the users rated.

B. Similarity based reccomendation: 

  1.  Recommender function is built step by step from scratch (Iteration 1):
   For example, imputing NaN's with 0, Cosine similarity matrix, targeting a single user at first and then generalizing the case to write a function for any user
  2.  Make a train-test split of the data and do the same (Iteration 2). Train the model and get predictions for test dataset
  3.  Compare the predictions and real values. Conduct several error analysis.
  4.  Visualize the comparisions

# Data
This dataset describes 5-star rating and free-text tagging activity from [MovieLens](http://movielens.org), a movie recommendation service. It contains 100836 ratings and 3683 tag applications across 9742 movies. These data were created by 610 users between March 29, 1996 and September 24, 2018. This dataset was generated on September 26, 2018.

Users were selected at random for inclusion. All selected users had rated at least 20 movies. No demographic information is included. Each user is represented by an id, and no other information is provided.

The data are contained in the files `links.csv`, `movies.csv`, `ratings.csv` and `tags.csv`. More details about the contents and use of all these files follows.

This is a *development* dataset. As such, it may change over time and is not an appropriate dataset for shared research results. See available *benchmark* datasets if that is your intent.

This and other GroupLens data sets are publicly available for download at <http://grouplens.org/datasets/>.
