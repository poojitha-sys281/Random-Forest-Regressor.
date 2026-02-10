# Random-Forest-Regressor.
# Random Forest Regressor – Used Car Price Prediction

##  Project Overview
This project uses a **Random Forest Regressor** machine learning model to predict the selling price of used cars. By analyzing important vehicle attributes such as age, present market value, fuel type, and usage history, the model provides accurate price estimations for the pre-owned automobile market.

---

##  Objectives
- Clean and preprocess the used car dataset  
- Perform feature engineering to calculate vehicle age  
- Encode categorical variables using One-Hot Encoding  
- Analyze correlations between vehicle features and selling price  
- Build and train a Random Forest Regressor model  
- Predict selling prices for used cars  

---

##  Technologies Used
- Python  
- Jupyter Notebook  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

##  Dataset Description
The dataset contains the following features used for prediction:

- **Selling_Price**: Price at which the car is sold (Target Variable)  
- **Present_Price**: Current ex-showroom price of the car  
- **Kms_Driven**: Total distance driven (in kilometers)  
- **Fuel_Type**: Petrol, Diesel, or CNG  
- **Seller_Type**: Dealer or Individual  
- **Transmission**: Manual or Automatic  
- **Owner**: Number of previous owners  
- **Year**: Manufacturing year of the car  

---

##  Methodology

### 1. Data Loading
- Imported the `car data.csv` dataset into the notebook

### 2. Feature Engineering
- Created a new feature **Current_Year**
- Calculated car age using:
- Removed unnecessary columns such as `Year` and `Car_Name`

### 3. Categorical Encoding
- Applied One-Hot Encoding to:
- Fuel_Type  
- Seller_Type  
- Transmission  
- Used `drop_first=True` to avoid multicollinearity

### 4. Data Visualization
- Used Seaborn Pairplot to visualize feature relationships  
- Created a correlation Heatmap to identify influential features

### 5. Model Training
- Split the dataset into training and testing sets  
- Trained a **Random Forest Regressor** to predict car selling prices  

---

##  Results
- **Present_Price** and **Car Age (no_of_years)** were identified as the most important factors  
- The Random Forest model effectively captured non-linear patterns  
- Produced accurate and reliable predictions for used car pricing  

---

##  How to Run the Project
1. Clone this repository  
2. Ensure `car data.csv` is available in the project directory  
3. Open the Jupyter Notebook  
4. Install dependencies:
5. Run all cells to preprocess data and train the model  

---

##  Conclusion
Random Forest Regression is highly effective for predicting used car prices. By incorporating key parameters such as present price, vehicle age, fuel type, and ownership details, the model delivers accurate price estimations that are valuable in the automotive resale market.

---

