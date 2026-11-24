# Bulldozer Price Prediction using Machine Learning

## About the Project

This project focuses on predicting the sale price of bulldozers using machine learning. The idea is to use information about previously sold bulldozers, such as their model, year of manufacture, equipment type and other features, to estimate how much a bulldozer might sell for.

I used the Bluebook for Bulldozers dataset from Kaggle and worked on understanding the data, handling missing values, training a model and evaluating its predictions.

## What I Did

- Explored the dataset to understand the different features and their relationship with sale prices.
- Analysed the sale price distribution and how prices changed over time.
- Converted the sale date into separate features such as year, month, day and day of the week.
- Split the data into training and validation sets based on the sale year.
- Handled missing numerical and categorical values.
- Converted categorical data into numerical values so it could be used by the machine learning model.
- Implemented a Random Forest Regressor to predict bulldozer prices.
- Used RandomizedSearchCV to find better model parameters.
- Compared the model's performance using MAE, RMSLE and R² scores.
- Generated predictions for the test dataset and exported them to a CSV file.
- Analysed feature importance to understand which factors had the most influence on the predicted prices.

## Results

The initial Random Forest model achieved a validation RMSLE of approximately **0.29**. After hyperparameter tuning using RandomizedSearchCV, the validation RMSLE improved to approximately **0.25**.

The feature importance analysis showed that factors like YearMade, ProductSize, saleYear and Enclosure played an important role in predicting bulldozer prices.

## Libraries Used

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Dataset

The project uses the Bluebook for Bulldozers dataset from Kaggle.

Dataset: https://www.kaggle.com/competitions/bluebook-for-bulldozers/data

The notebook uses the following files:

- `TrainAndValid.csv`
- `Test.csv`

Make sure the dataset files are placed in the appropriate `data` folder before running the notebook.

## How to Run

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```

3. Download the dataset from Kaggle.
4. Place the CSV files inside the `data` folder.
5. Open `Bulldozer-Price-Project.ipynb` in Jupyter Notebook.
6. Run the cells in order.

## Conclusion

Through this project, I got to work with a regression problem and understand how machine learning can be used to predict prices based on historical data. I also learned about feature engineering, handling missing values, time-based data splitting and hyperparameter tuning.

One thing I found interesting was how much the model's performance improved after tuning its parameters and how different bulldozer features contributed to the final predictions.

