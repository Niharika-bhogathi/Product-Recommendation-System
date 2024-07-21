# Product Recommendation System

## Project Description

This project focuses on building a comprehensive product recommendation system using collaborative filtering techniques. The dataset used is a collection of user ratings for electronic products. The main objective is to provide personalized product recommendations to users based on their past interactions and ratings.

## Dataset
Dataset Link : https://www.kaggle.com/datasets/vibivij/amazon-electronics-rating-datasetrecommendation?resource=download

The dataset used in this project is ratings_Electronics.csv, which contains the following columns:

user_id: Unique identifier for each user.

prod_id: Unique identifier for each product.

rating: Rating given by the user to the product (on a scale of 1 to 5).

timestamp: Timestamp of the rating (dropped for this analysis).

### Collaborative Filtering Methods
#### Rank-Based Recommendation System
1. Average Rating and Rating Count:
   
    Calculated for each product.

    Created a DataFrame with average ratings and count of ratings.

2. Top N Products Function:

    Function to recommend top N products based on highest average rating and minimum interactions.

    Recommendations for top 5 products with at least 50 and 100 interactions.

#### User-Based Collaborative Filtering

1. Similarity Calculation:

    Used cosine similarity to find similar users.

    Identified top 10 similar users to a given user.

2. Recommendation Function:
   
    Function to recommend products based on preferences of similar users.

    Recommendations for 5 products to specific users based on similarity scores.

#### Model-Based Collaborative Filtering using SVD

1. Sparse Matrix Conversion:

    Converted interaction matrix to a sparse matrix.

2. Singular Value Decomposition (SVD):
   
    Applied SVD on the sparse matrix.

    Constructed predicted ratings matrix.

3. Recommendation Function:

    Function to recommend products based on predicted ratings from SVD.

    Recommendations for top products to specific users.

#### Evaluation
Evaluated the SVD model using RMSE (Root Mean Squared Error).

Calculated and compared the average actual ratings and predicted ratings.
