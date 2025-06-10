
# Smart Movie Recommender System

## Overview
The *Smart Movie Recommender System* is designed to provide personalized movie suggestions using advanced machine learning techniques. It integrates *Demographic Filtering, Content-Based Filtering, and Collaborative Filtering* to generate accurate recommendations based on movie popularity, content similarity, and user preferences.

The system relies on various models such as *TF-IDF, CountVectorizer, Cosine Similarity, Linear Kernel, Singular Value Decomposition (SVD), and Cross-Validation* to enhance the recommendation process. Additionally, it utilizes the *IMDb Weighted Rating Formula*, ensuring that recommendations prioritize high-quality movies based on votes and ratings.

## Features
- *Demographic Filtering*: Identifies and ranks popular movies using metadata such as genre, votes, and ratings.
- *Content-Based Filtering*: Uses textual analysis methods to suggest movies similar to a user-selected film based on attributes like plot, keywords, and cast.
- *Collaborative Filtering*: Analyzes user interactions to predict preferences and suggest movies based on collective feedback from multiple users.

### Machine Learning Models & Techniques
To power the recommendation engine, the system employs:
- *TF-IDF (Term Frequency-Inverse Document Frequency)*: Processes textual movie descriptions to extract meaningful features.
- *CountVectorizer*: Converts movie metadata into numerical format for analysis.
- *Cosine Similarity & Linear Kernel*: Measures the closeness between different movie descriptions.
- *Singular Value Decomposition (SVD)*: Performs matrix factorization to enhance collaborative filtering predictions.
- *Cross-Validation*: Evaluates and fine-tunes model accuracy by testing multiple parameter configurations.

## IMDb Weighted Rating Formula
To refine the recommendation ranking, the system applies the *IMDb Weighted Rating Formula*:



![](https://image.ibb.co/jYWZp9/wr.png)




Where:
- *R* = The average rating of the movie.
- *v* = The number of votes for the movie.
- *m* = The minimum votes required for consideration.
- *C* = The mean rating across all movies.

This formula ensures that highly rated movies with sufficient votes are prioritized in recommendations, preventing bias toward lesser-known films with only a few high ratings.

## Dependencies
To run this project successfully, you need to install the following Python libraries:
- numpy: For numerical operations and handling data arrays.
- pandas: To process structured datasets efficiently.
- scikit-learn: Provides machine learning algorithms for filtering techniques.
- surprise: A specialized package for collaborative filtering.
- ast: Used to safely parse dataset components.
- jupyter notebook: A powerful interactive environment to run and visualize results.


## Future Improvements
Enhancements planned for future iterations:
- *Hybrid Recommender System*: Combining multiple filtering methods for more precise recommendations.
- *User Authentication & Preferences Tracking*: Allow users to create profiles and receive personalized suggestions.
- *Real-Time API Integration*: Connect the system with live movie databases for updated recommendations.


## Applications
- Personalized movie recommendations for streaming platforms
- Enhanced user experience by suggesting relevant content
- Hybrid recommendation approach for improved accuracy

##  Contributing
Contributions are welcomed! Feel free to submit pull requests to improve filtering techniques or optimize the recommendation engine.

