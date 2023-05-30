# MagnitudeMaster - Earthquake Magnitude Anticipation Project

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Overview

MagnitudeMaster is a project focused on earthquake magnitude anticipation. The goal of this project is to develop a model that can predict the magnitude of an earthquake based on various factors such as latitude, longitude, and timestamp. The project utilizes machine learning algorithms to build a predictive model.

## Code

The project code is provided in the `earthquake.ipynb` file. The code is implemented in Python and utilizes several libraries and frameworks, including:

- `numpy` for numerical computations
- `pandas` for data manipulation and analysis
- `matplotlib` and `plotly` for data visualization
- `datetime` and `pytz` for timestamp conversion
- `Basemap` from `mpl_toolkits.basemap` for creating a world map
- `MinMaxScaler` from `sklearn.preprocessing` for feature scaling
- `LazyRegressor` from `lazypredict.Supervised` for model evaluation
- Various regression models from `sklearn` and `lightgbm` libraries

## Getting Started

To get started with the project, follow the steps below:

1. Clone the repository: `git clone https://github.com/your-username/MagnitudeMaster.git`
2. Open the `earthquake.ipynb` file in a Jupyter Notebook environment.
3. Run the code cells in the notebook to execute the project code.

## Dataset

The project uses a dataset named `database.csv`. The dataset contains information about earthquakes, including attributes like date, time, latitude, longitude, depth, and magnitude. The dataset has 23,412 rows and 21 features. It also contains missing values, which are handled during data preprocessing.

## Data Preprocessing

The project performs various data preprocessing steps, including:

- Data overview: Displays the number of rows, number of features, feature names, missing values, and unique values in the dataset.
- Data subset selection: Selects a subset of relevant features from the dataset.
- Timestamp conversion: Converts the date and time columns into timestamp format.
- Correlation matrix visualization: Visualizes the correlation matrix of the dataset using a heatmap.
- Visualization of affected areas on a world map: Plots the latitude and longitude coordinates of earthquakes on a world map.

## Model Development and Evaluation

The project utilizes several regression models to predict earthquake magnitudes. The models are evaluated using the LazyRegressor, which provides insights into the performance of various models. The evaluation metrics used include adjusted R-squared, R-squared, root mean squared error (RMSE), and time taken for model training.

## Results

The LazyRegressor analysis provides the following results for the tested models:

```
Adjusted R-Squared   R-Squared   RMSE   Time Taken
-------------------------------------------------
HistGradientBoostingRegressor    0.02    0.02    0.42    0.35
LGBMRegressor                   0.02    0.02    0.42    0.25
GradientBoostingRegressor       0.02    0.02    0.43    3.14
...
```

The results show the performance of each model in terms of adjusted R-squared, R-squared, RMSE, and time taken for training. These metrics can be used to compare and select the best model for earthquake magnitude anticipation.

## Conclusion

MagnitudeMaster is a project that aims to anticipate earthquake magnitudes using machine learning techniques. By analyzing the provided dataset
