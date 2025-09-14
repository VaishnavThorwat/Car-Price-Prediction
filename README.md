# Car Price Prediction 🚗

## 1\. Executive Summary

This project focuses on building a machine learning model to accurately predict the selling price of used cars. The model is developed using a comprehensive dataset of various car features, including brand, body type, engine specifications, and mileage. Through data cleaning, exploratory data analysis (EDA), and the implementation of a **Decision Tree Regressor**, the project successfully creates a predictive tool that achieves a high $R^2$ score of approximately **0.887**. This indicates that the model can explain a significant portion of the variance in car prices, making it a valuable tool for stakeholders in the used car market.

-----

## 2\. Project Overview

The objective of this project is to create a data-driven solution for estimating the price of used cars. The used car market can be challenging for both buyers and sellers due to fluctuating prices and a wide range of influencing factors. By leveraging a dataset containing detailed car attributes, this project aims to train a robust regression model that can provide fair and reliable price predictions.

-----

## 3\. Data

The project utilizes the "CarPrice\_Assignment.csv" dataset.

  * **Source:** The dataset is provided in the project files.
  * **Size:** The dataset contains **205 entries** and **26 columns**.
  * **Key Features:**
      * `CarName`: The name of the car, which was preprocessed to extract only the company name.
      * `fueltype`: The type of fuel used by the car (e.g., gas, diesel).
      * `carbody`: The body style of the car (e.g., sedan, hatchback, wagon).
      * `enginetype`: The type of engine.
      * `enginesize`: The size of the car's engine.
      * `price`: The selling price of the car, which is the target variable for the prediction model.

-----

## 4\. Methodology

The project followed a standard machine learning pipeline:

1.  **Data Loading & Initial Exploration**: The dataset was loaded using `pandas`. Initial checks confirmed no missing or duplicate values.
2.  **Exploratory Data Analysis (EDA)**: The distribution of the `price` variable was visualized using `seaborn`, and a correlation heatmap was generated to understand relationships between features.
3.  **Data Preprocessing & Feature Engineering**: Categorical variables were converted into numerical dummy variables using `pandas.get_dummies()` to prepare the data for the model. The `car_ID` column was dropped as it was not relevant for the prediction task.
4.  **Model Training**: The data was split into training and testing sets (70/30). A **Decision Tree Regressor** from `sklearn` was chosen and trained on the preprocessed data.
5.  **Model Evaluation**: The model's performance was evaluated using two key metrics on the test set:
      * **Mean Absolute Error (MAE)**: A common metric for regression models.
      * **R-squared ($R^2$) Score**: The model achieved a score of **0.8866**. An $R^2$ score close to 1 indicates that the model explains a high proportion of the variance in the target variable.

-----

## 5\. Key Findings

  * The exploratory data analysis revealed the distribution of car prices and the correlation between various features.
  * The **Decision Tree Regressor** proved to be an effective choice for this problem, as shown by its high $R^2$ score.
  * The project successfully demonstrates how a machine learning model can be used to predict car prices based on a set of technical and categorical features.

-----

## 6\. Technologies/Libraries

  * **Programming Language:** Python
  * **Data Analysis:** `pandas`, `numpy`
  * **Data Visualization:** `seaborn`, `matplotlib.pyplot`
  * **Machine Learning:** `sklearn` (specifically `DecisionTreeRegressor`, `train_test_split`, `StandardScaler`, and `r2_score`)
  * **Notebook:** Jupyter Notebook

-----

## 7\. How to Use

To run the project locally, please follow these steps:

1.  Ensure you have Python installed.
2.  Clone the GitHub repository:
    ```bash
    git clone https://github.com/VaishnavThorwat/Car-Price-Prediction.git
    ```
3.  Install the necessary libraries listed in the `requirements.txt` file (if you have one) or by manually installing them.
4.  Navigate to the project directory and open the Jupyter Notebook:
    ```bash
    cd Car-Price-Prediction
    jupyter notebook
    ```
5.  Run all the cells in the `Task3_Car Price Prediction.ipynb` notebook in sequence to see the full analysis and model training process.

-----

## 8\. Contact

For any questions or feedback, please feel free to reach out.

  * **GitHub:** [VaishnavThorwat](https://github.com/VaishnavThorwat)
  * **LinkedIn:** [Vaishnav Thorwat](www.linkedin.com/in/vaishnav-thorwat)
