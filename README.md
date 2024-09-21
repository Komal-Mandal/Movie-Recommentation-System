# Movie-Recommentation-System

# Movie Recommentation System By Using Machine Learning

The system recommends movies based on user preferences using various recommendation algorithms.


## Acknowledgements

I would like to express my gratitude to the following resources and individuals who made this project possible:

MovieLens: For providing the comprehensive and widely-used dataset, which is essential for building recommendation systems.

scikit-learn and Surprise Libraries: For offering easy-to-use machine learning tools and collaborative filtering algorithms that formed the backbone of this project.

Stack Overflow and the developer community: For sharing insights, tutorials, and troubleshooting advice during development.

Kaggle Notebooks: For inspiration and guidance from various public notebooks and community contributions in the field of recommendation systems.

OpenAI’s GPT: For assisting in generating insightful responses and clarifying concepts during the project’s development.


## Features

1.Content-Based Filtering: Recommends movies similar to those the user has liked in the past, based on movie metadata such as genres, keywords, and descriptions.

2.Collaborative Filtering: Utilizes user-item interactions (such as ratings) to find users with similar preferences and recommend movies they liked.

3.Hybrid Model: Combines both content-based and collaborative filtering to improve accuracy.

## Appendix

1.TF-IDF Vectorization: This technique is used to convert text data (e.g., movie descriptions) into numerical form. It captures the importance of each word to represent the content of a movie.

2.Cosine Similarity: This metric is used to measure similarity between movies, based on the TF-IDF vectors.

3.Recommends movies by identifying patterns in user behavior (e.g., ratings).

4.Matrix Factorization (SVD): A collaborative filtering technique that decomposes the user-item interaction matrix into latent factors, enabling the system to predict ratings for unseen movies.

5.User-User and Item-Item Filtering: Finds similarities between users or movies and makes recommendations based on these similarities.

6.Combines content-based and collaborative filtering approaches by averaging the recommendations from both models or blending their predictions in different ways.

B. Evaluation Metrics

1.Mean Absolute Error (MAE):

Measures the average magnitude of the error between predicted ratings and true ratings. It’s useful for evaluating the accuracy of predicted movie ratings.

2.Root Mean Square Error (RMSE):

Measures the square root of the average squared differences between predicted and true ratings. It penalizes larger errors more than MAE.

3.Precision:
Measures the proportion of recommended movies in the top K that are relevant to the user.

4.Recall:
Measures the proportion of relevant movies that are successfully recommended to the user within the top K recommendations.

C. Data Preprocessing

1.Handling Missing Values:

If there are missing ratings or metadata, they are either removed or imputed (using methods like average rating for that user or genre).

2.Feature Extraction:

Genres: Each movie is associated with a list of genres, and these are converted into binary vectors.
Movie Descriptions/Keywords: Extracted and vectorized using TF-IDF.

3.Normalization:
User ratings are normalized (scaled to a consistent range) to ensure consistency in predictions.

D. Tools and Libraries
1.Python: Main programming language used for implementation.
2.Pandas: For data manipulation and analysis.
3.NumPy: For numerical computations.
4.scikit-learn: For building content-based filtering models and evaluation metrics.
5.Surprise: For implementing collaborative filtering algorithms, especially matrix 6.factorization (SVD).
6.Matplotlib/Seaborn: For data visualization.

E. Dataset Information
Description: The dataset includes user ratings for thousands of movies. It contains:
1.Movie Metadata: Movie titles, genres, release year, etc.
2.User Ratings: Users rate movies on a scale of 1 to 5.
3.User IDs: Anonymized user identifiers.

F. Hyperparameters

Latent Factors (Collaborative Filtering): The number of latent factors in matrix factorization (SVD). Common values range from 50 to 200.

Regularization: Used to prevent overfitting by penalizing large latent factors. Adjusted through cross-validation.

Learning Rate: For collaborative filtering models, controls the step size for updating latent factors during training.















