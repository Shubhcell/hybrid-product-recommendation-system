# hybrid-product-recommendation-system
Overview

This project implements a hybrid product recommendation system for an e-commerce dataset, combining content-based filtering and collaborative filtering. It processes a dataset of 29,972 products, cleans the data, generates synthetic user ratings, and builds a recommendation engine using TF-IDF vectorization, cosine similarity, and the SVD algorithm from the Surprise library. The system blends product similarity (based on features like name, description, and category) with user preferences to provide personalized recommendations.

The project is implemented in a Jupyter notebook (b.ipynb) and includes saved models and data for reuse in applications.

# Features





Data Preprocessing: Cleans an e-commerce dataset (out.csv) by handling missing values, converting data types, and selecting relevant features (e.g., product name, price, rating).



Content-Based Filtering: Uses TF-IDF vectorization and cosine similarity to recommend products based on textual features (name, description, tags, category, brand).



Collaborative Filtering: Generates synthetic user ratings for 100 users and uses SVD to predict user preferences.



Hybrid Recommendations: Combines content-based and collaborative filtering with a configurable weighting factor (alpha=0.6).

# Dataset

The project uses a product dataset (out.csv) with 32 columns, including:





Product Name, Product Description, Product Price, Product Rating, Product Category, Product Brand, Product Image Url, Product Tags, Product Url.



The dataset is cleaned and saved as cleaned_products12.csv.



Synthetic user ratings are generated for 100 users, each rating 10 products (1–5 scale), saved as synthetic_user_ratings.csv.
