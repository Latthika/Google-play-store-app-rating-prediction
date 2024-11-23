# Predicting Google Play Store App Ratings

## Objective:

This project aims to build a predictive model for estimating app ratings on the Google Play Store.  The model uses various app attributes like category, reviews, size, installs, and price to predict ratings.  Understanding these influencing factors helps developers optimize apps for higher customer satisfaction and platform visibility.

## Data Source:

[https://www.kaggle.com/datasets/muhammadarsalanakram/google-app-rating-prediction](https://www.kaggle.com/datasets/muhammadarsalanakram/google-app-rating-prediction)

## Dataset Description:

*   **App:** App name.
*   **Category:** App category.
*   **Rating:** User rating.
*   **Reviews:** Number of user reviews.
*   **Size:** App size in megabytes.
*   **Installs:** Number of app installs.
*   **Type:** Paid or free app.
*   **Price:** App price.
*   **Content Rating:** Content rating.
*   **Genres:** App genre.
*   **Last Updated:** Last update date.
*   **Current Ver:** Current app version.
*   **Android Ver:** Android version required.


## Project Workflow:

1. **Data Loading and Exploration:** The project begins by loading the dataset, exploring its structure, and understanding the distribution of key features.  Histograms, scatter plots, and pie charts visualize data distribution, revealing insights into app ratings, reviews, and other factors.

2. **Data Cleaning and Preprocessing:** Missing values are handled, and outliers are addressed to improve model accuracy.  Categorical features are converted using label encoding, and size values are transformed to numerical format. Data visualization helps identify key relationships between features.

3. **Feature Engineering:**  No additional feature engineering steps were performed in this particular implementation.

4. **Model Building:** Linear Regression, Random Forest Regressor, and Decision Tree Regressor models are trained and compared.

5. **Model Evaluation:** The models' performance is evaluated using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE) on a test set.  The Random Forest Regressor shows the best performance.

6. **Prediction Function:** A `predict_rating` function demonstrates how to use the trained models to predict ratings for new app data.

7. **Database Integration:** The processed dataset is saved to a SQLite database for persistent storage and later retrieval or analysis.


## Key Findings:

*   Most apps receive ratings between 4.0 and 4.5.
*   Apps with more reviews tend to have higher ratings.
*   The vast majority of apps on the Google Play Store are free.
*   Communication, Social, and Productivity apps have the highest number of installs.


## Next Steps:

*   Explore more sophisticated feature engineering techniques.
*   Experiment with additional machine learning algorithms and hyperparameter tuning.
*   Investigate the impact of "Last Updated" and other time-based features on ratings.
*   Analyze app reviews for sentiment analysis and incorporate text-based features.


