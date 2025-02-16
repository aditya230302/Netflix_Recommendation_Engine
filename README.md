# Netflix_Recommendation_Engine

## Dataset Information

![{47BCFE8E-682C-4FEC-9C6E-B557F2D05FEA}](https://github.com/user-attachments/assets/c2350645-5e1d-4ef5-bb30-570b10a404c2)

- The numbers with " : " behind them and NaN in corresponding rating are movie ids according to data set
- The rest are customer id

## Objective

![image](https://github.com/user-attachments/assets/2f1c6f3e-52cb-4489-a4f8-8aa65cbfae24)


**Importing Surprise Library**

The Surprise library is a Python library used for building and analyzing recommender systems. It is particularly useful for collaborative filtering-based recommendation algorithms. Surprise stands for "Simple Python Recommendation System Engine" and is designed to work efficiently with large datasets.

📌 Key Features of Surprise:
- Implements collaborative filtering methods (e.g., matrix factorization and nearest neighbors algorithms).
- Supports both explicit (e.g., ratings) and implicit feedback.
- Provides tools for model evaluation (e.g., RMSE, MAE, precision-recall).
- Allows for custom algorithms to be implemented.
- Works well with pandas and scikit-learn.


📌 **1. Reader (Data Preprocessing)**

The Reader class defines the rating scale and format of the dataset. Since different datasets have different rating scales (e.g., 1–5 stars or 0–10 scores), the Reader ensures that Surprise understands the data correctly.
- If using a custom dataset, you must specify the Reader while loading data.
- If using built-in datasets (like ml-100k), the Reader is not required.

📌 **2. Dataset (Loading Data)**

The Dataset module is used to load and process recommendation data.

📌 **3. SVD (Singular Value Decomposition)**

SVD (Singular Value Decomposition) is a matrix factorization algorithm that is widely used in recommendation systems.
- A collaborative filtering algorithm used for making recommendations

**SVD (Singular Value Decomposition) in a recommendation system works by finding patterns in user preferences and item similarities. Here's a basic idea without going deep into the topic**

**1) What the System Has:** A big table (matrix) with users on one side and items (like movies) on the other. Users give ratings to items, but not everyone has rated everything

**2) What SVD Does**: SVD looks at the ratings that are available and tries to figure out the hidden connections between users and items. It learns what kind of movies users like based on their previous ratings

**3) How It Helps:** Once SVD understands these patterns, it can predict how a user might rate a movie they haven’t seen yet. Based on these predictions, the system recommends movies that the user is most likely to enjoy

**4) Step-by-Step Implementation of SVD in a Recommendation System**

Install and Import Libraries

Load and Prepare the Dataset

Train the SVD Model

Evaluate the Model

Make Predictions
