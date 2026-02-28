# 🏠 California Housing Price Prediction using Linear Regression

## 📖 Overview
This project demonstrates a complete workflow for building a **Linear Regression** model to predict **median house values** in California districts using the California Housing dataset from `scikit-learn`.  
The workflow includes **data loading, preprocessing, train-test splitting, scaling, model training, cross-validation, prediction, and evaluation**.

## 📊 Dataset
- **Dataset:** California Housing (`sklearn.datasets.fetch_california_housing`)
- **Instances:** 20,640
- **Features:** 8 numeric features
- **Target:** `MedHouseVal` – Median house value in hundreds of thousands of dollars

**Features:**
| Feature      | Description                                      |
|-------------|--------------------------------------------------|
| MedInc      | Median income in block group                     |
| HouseAge    | Median house age in block group                  |
| AveRooms    | Average number of rooms per household            |
| AveBedrms   | Average number of bedrooms per household         |
| Population  | Block group population                            |
| AveOccup    | Average number of household members             |
| Latitude    | Block group latitude                             |
| Longitude   | Block group longitude                            |

## 🛠 Technology Used

- **Programming Language:** Python 3.11 🐍
- **Data Handling:** pandas, numpy 🗃️
- **Machine Learning:** scikit-learn 🤖
- **Data Visualization:** matplotlib, seaborn 📈
- **IDE/Environment:** JupyterLab 💻

## 🏗 Project Workflow

1. **Import Libraries**  
   - `numpy`, `pandas` for data handling  
   - `matplotlib`, `seaborn` for visualization  
   - `sklearn` for ML models, preprocessing, and metrics  

2. **Load Dataset**  
   - Fetch the California Housing dataset using `fetch_california_housing()`  
   - Convert dataset features into a pandas DataFrame  
   - Assign proper column names using `housing.feature_names`  

3. **Separate Features and Target**  
   - `X` contains feature columns  
   - `y` contains the target variable (`MedHouseVal`)  

4. **Train-Test Split**  
   - Split dataset into training (70%) and test (30%) sets  
   - `random_state=42` ensures reproducibility  

5. **Data Standardization**  
   - Standardize feature values using `StandardScaler`  
   - Fit on training data and transform both training and test sets  

6. **Linear Regression Model**  
   - Initialize and train a `LinearRegression` model on the standardized training data  

7. **Cross-Validation**  
   - Evaluate model stability on training set using **7-fold cross-validation**  
   - Compute **negative mean squared error (MSE)** for each fold  
   - Calculate average MSE  

8. **Prediction & Evaluation**  
   - Predict house values on test data  
   - Visualize residuals using `seaborn` KDE plot  
   - Evaluate model performance using **R² score**  

## 📈 Results

- Model performance is evaluated using **R² score** and **MSE**.  
- Residuals are visualized to understand prediction errors.

## 👨‍💻 Author & Contact

- **Name:** Akisha Bhujel  
- **GitHub:** [akisavujel](https://github.com/akisavujel) 🐱  
- **LinkedIn:** [akishabhujel](https://www.linkedin.com/in/akishabhujel/) 💼  
- **Kaggle:** [akisavujel](https://www.kaggle.com/akisavujel) 🏆  
- **Email:** akishabhujel@example.com 📧
