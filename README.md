# Multiple-Linear-Regression-Housing-Price-Prediction
Machine Learning project using Multiple Linear Regression to predict house prices based on property features such as area, bedrooms, bathrooms, stories, parking, location, amenities, and furnishing status.


# Multiple Linear Regression - Housing Price Prediction

## Project Overview

This project uses **Multiple Linear Regression** to predict house prices based on various property features.

The project demonstrates a complete machine learning workflow, including data loading, data exploration, preprocessing, categorical variable encoding, train-test splitting, model training, evaluation, visualization, and interpretation of model coefficients.

## Objective

The main objective of this project is to build a Multiple Linear Regression model that can predict house prices using different property characteristics.

## Dataset

The project uses a housing dataset containing **545 records** with the following features:

* `price` - House price
* `area` - Property area
* `bedrooms` - Number of bedrooms
* `bathrooms` - Number of bathrooms
* `stories` - Number of stories
* `mainroad` - Whether the property is connected to the main road
* `guestroom` - Whether the property has a guest room
* `basement` - Whether the property has a basement
* `hotwaterheating` - Whether hot water heating is available
* `airconditioning` - Whether air conditioning is available
* `parking` - Number of parking spaces
* `prefarea` - Whether the property is located in a preferred area
* `furnishingstatus` - Furnishing status of the property

## Machine Learning Algorithm

### Multiple Linear Regression

Multiple Linear Regression is used to model the relationship between the house price and multiple independent variables.

The model uses several property characteristics simultaneously to estimate the expected house price.

## Data Preprocessing

The following preprocessing steps are performed:

1. Load the dataset using Pandas.
2. Check the dataset for missing values.
3. Handle missing values if required.
4. Convert categorical variables into numerical variables using **One-Hot Encoding**.
5. Separate the input features (`X`) and target variable (`y`).

Categorical variables such as `mainroad`, `guestroom`, `basement`, `airconditioning`, `prefarea`, and `furnishingstatus` are converted into numerical features.

## Features Used

The model uses:

* Area
* Bedrooms
* Bathrooms
* Stories
* Parking
* Main road
* Guest room
* Basement
* Hot water heating
* Air conditioning
* Preferred area
* Furnishing status

The target variable is:

* **House Price (`price`)**

## Model Training

The dataset is divided into:

* **80% Training Data**
* **20% Testing Data**

The model is trained using the training dataset and then used to predict house prices for the testing dataset.

## Model Evaluation

The model performance is evaluated using:

### Mean Squared Error (MSE)

MSE measures the average squared difference between the actual house prices and the predicted house prices.

### R-squared (R²)

R² measures how well the model explains the variation in house prices.

The notebook calculates both MSE and R² on the test dataset.

## Visualization

The project includes an **Actual vs. Predicted House Prices** scatter plot.

This visualization helps compare the actual house prices with the values predicted by the Linear Regression model.

## Model Interpretation

The project also calculates the **coefficients (slopes)** and **intercept** of the Linear Regression model.

The coefficients help understand the impact of each input feature on the predicted house price.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook

## Project Structure

```text
Multiple-Linear-Regression-Housing-Price-Prediction/
│
├── Multiple-LR-Housing-Dataset.ipynb
├── Model-Evaluation-California-Housing-Prices_.ipynb
├── Housing.csv
└── README.md
```

## How to Run the Project

### 1. Install Python

Make sure Python is installed on your system.

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open the Notebook

Open:

```text
Multiple-LR-Housing-Dataset.ipynb
```

Make sure `Housing.csv` is in the same folder as the notebook.

### 5. Run the Notebook

Run the cells from top to bottom.

## California Housing Model Evaluation

The repository also contains a separate notebook:

```text
Model-Evaluation-California-Housing-Prices_.ipynb
```

This notebook uses the **California Housing dataset** available through Scikit-learn and evaluates a Linear Regression model using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R-squared (R²)

It also includes an Actual vs. Predicted House Prices visualization.

## Conclusion

This project demonstrates how Multiple Linear Regression can be applied to a real-world housing dataset to predict house prices using multiple property characteristics.

It also demonstrates important machine learning concepts such as categorical data preprocessing, feature selection, model training, evaluation, visualization, and model interpretation.

## Author

**Gowtham V**

## License

This project is intended for educational and portfolio purposes.
