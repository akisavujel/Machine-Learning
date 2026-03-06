# 🏡 California Housing Price Prediction 👶

Predicting California housing prices using Decision Tree Regression and GridSearchCV to optimize model performance. This project demonstrates data preprocessing, regression modeling, hyperparameter tuning, evaluation, and visualization in Python.

![California Housing Dataset Preview](https://github.com/akisavujel/Machine-Learning/blob/20f2c12895e6858dc36fbb038b91dda93a30d340/Day-5/Cross-Valid/Images/Housing-Regression.png) 👶

## 📂 Dataset 🍼
The dataset is the **California Housing Dataset** from scikit-learn:

- **Number of instances:** 20,640  
- **Number of features:** 8 numeric attributes  
- **Target variable:** Median house value (`MedHouseVal`) in $100,000  
- **Features:**
  1. `MedInc` — Median income in block group
  2. `HouseAge` — Median house age
  3. `AveRooms` — Average number of rooms per household
  4. `AveBedrms` — Average number of bedrooms per household
  5. `Population` — Block group population
  6. `AveOccup` — Average number of household members
  7. `Latitude` — Block group latitude
  8. `Longitude` — Block group longitude  

![California Housing Dataset Preview](https://github.com/akisavujel/Machine-Learning/blob/20f2c12895e6858dc36fbb038b91dda93a30d340/Day-5/Cross-Valid/Images/Dataset-Overview.png) 👶

## 🛠 Tools & Libraries 🧸
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn 

## 📊 Methodology 🚀
1. **Data Loading & Exploration**  
   Load the California Housing dataset and explore the features and target distribution.  

2. **Train-Test Split**  
   Split data into training and testing sets (80%-20%).

3. **Decision Tree Regression**  
   Train a baseline Decision Tree Regressor on the dataset.

4. **Model Evaluation**  
   Evaluate using Mean Squared Error (MSE) and R² score.  

5. **Hyperparameter Tuning with GridSearchCV**  
   Optimize the Decision Tree by testing different `max_depth`, `criterion`, `splitter`, and `max_features` parameters.  

6. **Visualization**  
   Visualize predictions vs actual values and feature importance.

## ⚡ Results ✨

**Basic Decision Tree Regressor**  
- Mean Squared Error: 0.505  
- R² Score: 0.614  

**GridSearchCV Decision Tree Regressor**  
- Mean Squared Error (MSE): 0.437  
- R² Score: 0.594  
- Best Hyperparameters:  
  - `max_depth`: 8  
  - `criterion`: squared_error  
  - `splitter`: best  
  - `max_features`: auto  

## 🎨 Dashboard / Visuals 🎈
- HTML and CSS used for **notebook dashboard** presentation.  
- Cards with metrics, feature importance, and dataset overview.  
- Interactive visualization of predictions vs actual values.  

## 💡 Insights 🌱
- GridSearchCV tuning improved the model's MSE.  
- `MedInc` (median income) is the most significant feature.  
- Future improvements: try **Random Forest or Gradient Boosting** for better performance.

## 📌 Author 🎀
**Akisha Bhujel** &nbsp; | &nbsp; [Kaggle](https://www.kaggle.com/akisavujel) &nbsp; | &nbsp; [GitHub](https://github.com/akisavujel) &nbsp; | &nbsp; [LinkedIn](https://www.linkedin.com/in/akishabhujel/)  

Thank you for viewing this project! 🙏👶
