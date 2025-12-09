# Fantasy Football Performance Predictor

## Project Overview
This project applies Deep Learning techniques to solve a common problem in sports analytics: predicting fantasy football performance. By training a Multi-Layer Perceptron (MLP) on quarterback statistics and defensive rankings, this tool quantifies the expected point output for a player, helping managers optimize their starting lineups.

## Key Features
* **Deep Learning Model:** A custom Keras Sequential model with Dense and Dropout layers.
* **Exploratory Data Analysis (EDA):** Visualizations of feature correlations and target variable distributions.
* **Data Pipeline:** Includes a synthetic data generator to simulate NFL statistics for reproducible testing.
* **Performance Metrics:** Evaluates the model using R-Squared ($R^2$), Mean Squared Error (MSE), and Mean Absolute Error (MAE).

## Technologies Used
* **Language:** Python 3.11
* **Libraries:** TensorFlow, Keras, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## Results
The model successfully captures the non-linear relationship between raw stats (Yards/TDs) and fantasy points, achieving an $R^2$ score of **0.9312** on the test set. EDA confirmed that while volume stats drive performance, defensive matchups introduce significant variance that the neural network learns to predict.