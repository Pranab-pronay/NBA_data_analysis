# NBA Game Outcome and Lineup Prediction

## Overview
This project aims to predict the outcome of NBA games and recommend the best player lineups using machine learning techniques. We utilize historical NBA game data to train various models and provide insights into optimal player combinations and game results.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [Contributors](#contributors)
- [License](#license)

## Introduction
Predicting the outcome of NBA games and identifying optimal player lineups is a complex task that can provide significant value to coaches, analysts, and sports enthusiasts. This project employs machine learning techniques, including Random Forest Classifier, Multi-Layer Perceptron (MLP), K-Nearest Neighbors (KNN), and Decision Tree Classifier to analyze NBA game data and make predictions.

## Dataset
The dataset used in this project spans NBA games from 2007 to 2012, including features such as:
- Player performance metrics (e.g., points scored, rebounds, assists)
- Team statistics (e.g., win-loss record, offensive and defensive efficiency)
- Game conditions (e.g., venue, date, opponent)
- Lineup details (e.g., player names, starting and ending minutes)

## Feature Engineering
Feature engineering was a critical step in this project. Key techniques included:
- Customized encoding for player names to handle the large number of categorical variables.
- Correlation matrix analysis to identify the most relevant features for outcome prediction.
- Handling class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).
- Normalizing data with Standard Scaler to ensure model robustness.

## Modeling
We implemented and evaluated the following machine learning models:
- **Random Forest Classifier**: Our baseline model known for its robustness and accuracy in classification tasks.
- **Multi-Layer Perceptron (MLP) Classifier**: An artificial neural network model capable of learning complex patterns.
- **K-Nearest Neighbors (KNN)**: A simple, yet effective, instance-based learning algorithm.
- **Decision Tree Classifier**: A model that uses tree-like structures to make decisions based on feature values.

## Results
### Outcome Prediction
- **Random Forest Classifier**: Highest accuracy with an F1 Score of 0.71.
- **MLP Classifier**: Good performance with an accuracy of 0.65.
- **KNN and Decision Tree**: Lower accuracy compared to Random Forest and MLP.

### Lineup Prediction
- **Random Forest Classifier**: Best performance with accuracy and F1 Score of 0.78 and 0.58, respectively.
- **MLP Classifier**: Moderate performance with accuracy of 0.63 and F1 Score of 0.43.
- **KNN and Decision Tree**: Lower performance compared to Random Forest.

## Usage
To run the project, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Pranab-pronay/NBA_data_analysis.git
    cd NBA_data_analysis
    ```

2. **Install the necessary dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter notebooks**:
    - `1.Outcome_prediction.ipynb`: Contains the code for predicting game outcomes.
    - `2.Lineup_prediction.ipynb`: Contains the code for predicting player lineups.


4. **Dataset**:
   Ensure the dataset file (`matchups-2012.csv`) is placed in the project directory.


5. **Test the Model**:
   You can test the model by editing the `test.csv` file. Modify the player names and other relevant features to see the outcome predictions and recommendations for the best 5th player.
    - To predict game outcomes, edit the player names and game features in `test.csv`.
    - To get recommendations for the best 5th player, modify the relevant features in `test.csv` and rerun the notebook.

## Contributors
- Pranab Datta ([pranab.datta@ontariotechu.net](mailto:pranab.datta@ontariotechu.net))
- Jahnavi Adla ([adla.jahnavi@ontariotechu.net](mailto:adla.jahnavi@ontariotechu.net))
