# steam-game-recommender

created by Sean Hingco
  18 June, 2021
 
 
Uses kaggle's "Steam Video Games" dataset and k-nearest neighbors to 
recommend up to 5 different video games from the Stean Library based on user input.
Borrows heavily from Kevin Liao's "Prototyping a Recommender System Step by Step Part 1: KNN Item-Based Collaborative Filtering"
on Towards Data Science (https://towardsdatascience.com/prototyping-a-recommender-system-step-by-step-part-1-knn-item-based-collaborative-filtering-637969614ea"),
as well as Susan Li's "Building A Book Recommender System – The Basics, kNN and Matrix Factorization" on DataScience+ (https://datascienceplus.com/building-a-book-recommender-system-the-basics-knn-and-matrix-factorization/).

Features:
  - takes user input to generate knn model
  - uses hours played to determine rating
  - returns 5 games and distance from user input
  - requires installation of Jupyter


Possible Future Updates and Additions:
  - autocomplete feature for quality of life change
  - web app option for easier use


Downfalls: This approach is based off the assumption that users will play a game for longer hours the more they like it.
This method is inherently flawed, as hours played cannot always be correlated to rating. Some games may simply have less gameplay available
even if a user really likes the games. As a result, many games which may be a solid candidate for recommendation will not be recommended due
to limited gameplay available. 
