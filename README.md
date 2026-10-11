# House Price Prediction Using Machine Learning

## Project Overview

This project predicts house prices using **Linear Regression** based on housing features such as area, number of rooms, build year, location, street type, furnishing, property type, and pool availability.

## Objective

To build a machine learning model that learns from housing data and predicts the price of a house from its property attributes.

## Dataset

The project uses `Housing_Dataset.csv`.

**Input Features:**

* `Area_SqFt`
* `Rooms`
* `Build_Year`
* `Location`
* `Street_Type`
* `Furnishing`
* `Property_Type`
* `Has_Pool`

**Target Variable:** `Price`

Make sure `Housing_Dataset.csv` is in the same folder as the notebook before running the project.

## Technologies and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* Jupyter Notebook or Google Colab

## Project Workflow

1. Load and explore the housing dataset.
2. Check dataset information and missing values.
3. Visualize house-price distribution and the relationship between area and price.
4. Separate input features (`X`) and target variable (`y`).
5. Split the data into training and testing sets.
6. Handle missing numerical values using the median.
7. Handle missing categorical values using the most frequent value.
8. Scale numerical features using `StandardScaler`.
9. Encode categorical features using `OneHotEncoder`.
10. Train a Linear Regression model using a preprocessing pipeline.
11. Predict prices for the test dataset.
12. Evaluate the model using Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² score.
13. Use the trained model to predict the price of a new house.

## How to Run

1. Download or clone this project.

2. Keep `Housing_Dataset.csv` and `House_Price_Prediction.ipynb` in the same folder.

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scikit-learn jupyter
   ```

4. Open the notebook in Jupyter Notebook or upload it to Google Colab.

5. Run the notebook cells in order.

## Model

The project uses **Linear Regression**. A Scikit-learn `Pipeline` combines preprocessing and model training so that the same transformations are applied when making predictions. Numerical and categorical features are handled separately using a `ColumnTransformer`.

## Evaluation Metrics

* **MSE (Mean Squared Error):** Measures the average squared difference between actual and predicted prices.
* **RMSE (Root Mean Squared Error):** Expresses prediction error in the target variable's units.
* **R² Score:** Indicates how well the model explains variation in house prices.

The actual scores depend on the dataset and the train-test split. Run the notebook to see the results.

## Example Prediction

The notebook can create a new-house input with values such as area, rooms, build year, location, street type, furnishing, property type, and pool availability, then use the trained model to predict its price. Use category values that match those in the dataset.

## Project Files

* `House_Price_Prediction.ipynb` — notebook containing data exploration, preprocessing, model training, evaluation, and prediction.
* `Housing_Dataset.csv` — housing dataset used by the notebook.
* `README.md` — project documentation.

## Conclusion

This project demonstrates a basic end-to-end regression workflow, including data exploration, preprocessing, model training, evaluation, and prediction of house prices.

## Author

Add your name here.
