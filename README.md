# Random-Forest-Regressor.
Used Car Price Prediction using Random Forest Regressor
## Project Overview
This project implements a Random Forest Regressor model to predict the selling price of used cars. By analyzing various vehicle attributes—such as the car's age, current market value, and usage history—the model provides accurate price valuations to assist in the pre-owned automobile market.
--
## Objectives
To process and clean the used car dataset

To perform feature engineering (calculating vehicle age)

To handle categorical variables using One-Hot Encoding

To analyze the correlation between vehicle features and selling price

To build and train a Random Forest Regressor for price prediction
--
## Technologies Used
Python

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn
---
##Dataset Description
The dataset contains the following parameters (features) used to predict the Selling_Price:

Selling_Price: The price at which the car is being sold (Target Variable).

Present_Price: The current ex-showroom price of the car.

Kms_Driven: The total distance the car has been driven in kilometers.

Fuel_Type: The type of fuel used (Petrol, Diesel, CNG).

Seller_Type: Defines if the seller is a Dealer or an Individual.

Transmission: The gear transmission type (Manual or Automatic).

Owner: The number of previous owners the car has had.

Year: The manufacturing year of the car (used to calculate the car's age).
--
## Methodology
Data Loading: Importing the car data.csv file.

Feature Engineering:

Created a new feature Current_Year and no_of_years to quantify the car's age.

Formula: no_of_years = Current_Year - Year.

Dropped the original Year and Car_Name columns as they were no longer needed.

Categorical Encoding:

Applied One-Hot Encoding to convert Fuel_Type, Seller_Type, and Transmission into numerical values.

Utilized drop_first=True to prevent multicollinearity (Dummy Variable Trap).

Data Visualization:

Used Seaborn Pairplot to visualize relationships between parameters.

Generated a Heatmap to analyze the correlation between features like Present_Price and Selling_Price.
--
## Model Training:

Split the data into training and testing sets.

Trained the Random Forest Regressor to predict the final selling price.
--
## Results
The model identified Present_Price and Car Age (no_of_years) as the most significant factors influencing the selling price.

The Random Forest Regressor successfully captured non-linear relationships, providing robust predictions for used car valuations.
--
## How to Run the Project
Clone this repository

Ensure car data.csv is in the project directory

Open the Jupyter Notebook

Install dependencies: pip install pandas numpy matplotlib seaborn scikit-learn

Run all cells to process the data and train the model

## Conclusion
Random Forest Regression is highly effective for pricing used cars. By considering key parameters like the car's present price, age, and fuel type, the model delivers accurate estimates that are crucial for decision-making in the automotive resale market.
--
