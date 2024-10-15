# Movie Recommendation System

## Project Overview

This project is focused on building a movie recommendation system. The system uses various machine learning techniques to suggest movies to users based on their past ratings or preferences. The goal is to enhance user experience by recommending movies that they are more likely to enjoy.

## Dataset

The dataset used includes user ratings for a variety of movies. The key columns in the dataset are:

- **UserID**: The ID of the user.
- **MovieID**: The ID of the movie.
- **Rating**: The rating given by the user to a specific movie.
- **Timestamp**: The time when the rating was provided.

## Key Features

The system is designed to:

1. **Preprocess the Data**:
    - Handle missing values.
    - Normalize the data for better prediction accuracy.
    - Feature engineering to improve the model's performance.

2. **Model Training**:
    - **Collaborative Filtering**: The recommendation system uses collaborative filtering to predict ratings for movies a user hasn't watched yet based on the preferences of other users.
    - **Matrix Factorization**: This technique is employed to reduce the dimensionality of the dataset and improve model performance.

3. **Prediction**:
    - The trained model predicts the rating a user would give to a movie they haven't seen before, and recommends the top-rated movies.

## Installation and Setup

To run the movie recommendation system, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/borakgul/ML-Recommended-System-Design-w-TensorFlow
    ```

2. **Install the required dependencies**:
    The required Python libraries are listed in the `requirements.txt` file. You can install them by running:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter Notebook**:
    Start the notebook to explore the data and model.
    ```bash
    jupyter notebook MovieRecommendation.ipynb
    ```

## How It Works

1. **Data Preprocessing**:
    - The raw movie rating data is cleaned and preprocessed to remove any missing or irrelevant entries. 
    - Features are engineered to improve the prediction accuracy.

2. **Model Training**:
    - The system uses a **collaborative filtering** algorithm to predict movie ratings. 
    - Matrix factorization techniques are employed to reduce data dimensionality, which helps in better recommendations.

3. **Recommendations**:
    - Once the model is trained, it can recommend movies based on users' past preferences. It does this by finding similar users or movies and predicting ratings that the user might give.

## Results

The system recommends movies based on predicted ratings. For example:
- User A might get a recommendation for movies they have not seen yet, but which have been highly rated by users with similar preferences.
- The system is capable of making real-time predictions when new data is added.

## Technologies Used

- **Python** for data analysis and model building.
- **Pandas** and **NumPy** for data manipulation.
- **Scikit-learn** for building machine learning models.
- **Jupyter Notebook** for interactive code development.
  
## Future Improvements

- Add a **content-based recommendation system** to enhance the user experience.
- Improve the system's scalability to handle larger datasets.
- Implement a real-time recommendation engine.

## Conclusion

This project demonstrates how machine learning techniques can be used to build a personalized movie recommendation system. It highlights the power of collaborative filtering and matrix factorization in creating accurate movie recommendations.

