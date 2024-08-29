# NHL Game Outcome Prediction using Machine Learning
Final Project for Ironhack

## Project Overview

This project aims to predict the outcomes of NHL games using various machine learning models. The process involves gathering in-game data, selecting relevant features, and comparing different models to determine the best approach for predicting game results. The final model is then used to forecast the outcomes of playoff matchups.

## Objectives

The project follows these key steps:

1. Gather sufficient in-game data.
2. Run models on the data.
3. Pick the best/most appropriate model.
4. Use the selected model to predict future matchups (e.g., playoffs).

## Data Gathering

Data was collected using a free API due to the lack of readily available CSV files. The data collection was a two-step process:

1. **Getting Game IDs**: Game IDs were collected for the 2022-2023 and 2023-2024 NHL seasons.
2. **Pulling Game Stats**: For each Game ID, individual game statistics were pulled and stored in a dataframe.

### Challenges in Data Gathering

- **API Limitations**: The free API allowed only 1,000 calls, requiring multiple accounts to gather all necessary data.
- **Time Constraints**: The API requests were spaced out with a time interval to avoid being blocked.

## Feature Selection

After collecting the data, irrelevant information was removed, and features most relevant to predicting game outcomes were selected. These features included various in-game statistics, with the game result being the target variable.

## Models Used

Three machine learning models were tested:

1. **Linear Regression**: Achieved 95% accuracy.
2. **K-Nearest Neighbors (KNN)**: Achieved 89% accuracy with `n=22`.
3. **Random Forest Classifier**: Achieved 96.5% accuracy.

### Model Selection

Although the Random Forest Classifier had the highest accuracy, the project ultimately chose the Linear Regression model due to its interpretability and sufficiently high accuracy.

## Overfitting Check

The models were evaluated for overfitting by comparing their performance on training and testing datasets. The selected model performed well on both, indicating it generalizes well to unseen data.

## Challenges Faced

- **Feature Imbalance**: When predicting playoff outcomes, an imbalance in the number of features for home and away teams caused erroneous predictions.
- **Resolution**: The solution involved using aggregated statistics for the home team only, which avoided the issue of variable imbalance and allowed the model to run correctly.

## Future Improvements

The project identified the need to use comprehensive game analytics applied consistently to eliminate any imbalances or inconsistencies in the data, ensuring accurate predictions.

## The Team

- **Martin Krizan** - Data Analyst
- **Marty Krizany** - Hockey Enthusiast
- **Martinius Krizanius** - Data Spelunker
- **Morton Krozon** - API Abuser

## Conclusion

This project demonstrated the process of using machine learning to predict NHL game outcomes, with a focus on data gathering, feature selection, and model comparison. The Linear Regression model was chosen for its balance of accuracy and interpretability, and future work will address the challenges encountered in playoff prediction scenarios.

## Contact

For further information or collaboration, feel free to reach out to me at [Your Email] or connect with me on [LinkedIn Profile Link].

