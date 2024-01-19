# Linear-Classification-Models

**Mobile Price Classification**

## Overview
This project involves the analysis and prediction of mobile phone price ranges based on various features. The dataset used is `mobile_data.csv`, which includes several attributes of mobile phones.

## Dependencies
To run this project, the following Python libraries are required:
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Seaborn

## Dataset
The dataset `mobile_data.csv` contains various features of mobile phones, such as battery power, clock speed, RAM, etc., along with their price ranges.

## Features
The dataset includes the following features:
- `battery_power`
- `blue`
- `clock_speed`
- `dual_sim`
- `fc`
- `four_g`
- `int_memory`
- `m_dep`
- `mobile_wt`
- `n_cores`
- `pc`
- `px_height`
- `px_width`
- `ram`
- `sc_h`
- `sc_w`
- `talk_time`
- `three_g`
- `touch_screen`
- `wifi`
- `price_range`

## Data Processing Steps
1. **Import Libraries**: Necessary Python libraries are imported.
2. **Read Dataset**: The dataset is read into a pandas DataFrame.
3. **Check for Null Values**: The dataset is checked for any null values.
4. **Feature Selection**: Features correlating with `price_range` are identified and selected.
5. **Data Visualization**: 
   - Heatmap for correlation between features.
   - Histogram of `price_range`.
   - Histogram showing the relationship between `price_range` and `ram`.
6. **Data Scaling and Splitting**: The data is scaled using `StandardScaler` and split into training and test sets.

## Models
Two classification models are used to predict the price range:
1. **Logistic Regression**
   - Fitted on the training dataset.
   - Evaluated using a confusion matrix.
   - Trained using cross-validation.
2. **K-Nearest Neighbors (KNN)**
   - Fitted and evaluated for a range of `n_neighbors` values.
   - Best value of `k` is determined.
   - Trained using cross-validation.

## Results and Comparison
- The performance of Logistic Regression and KNN models is compared using a correlation matrix of their predictions.

## Usage
To use this code:
1. Ensure all dependencies are installed.
2. Place `mobile_data.csv` in the data directory.
3. Run the Python script to perform the analysis and view the model predictions.

## Note
The script contains detailed comments and instructions for each section of the code for better understanding and ease of navigation.
