# Flight Data Classification using Support Vector Machine Kernels

## Project Overview
This project applies Support Vector Machine (SVM) classification models to airline flight data to analyze and predict flight-related outcomes. The project includes two machine learning tasks: flight price classification and flight destination classification.

The main goal is to compare different SVM kernels and understand how model performance changes across linear and nonlinear classification methods. The project demonstrates data preprocessing, feature selection, model training, kernel comparison, accuracy evaluation, and decision boundary visualization using Python.

## Objectives
The objectives of this project are to:

- Analyze airline flight data using Python
- Prepare numerical features for machine learning models
- Build SVM classification models using different kernels
- Compare model performance across Linear, RBF, Polynomial, and SVC models
- Predict flight-related classes using selected features
- Visualize decision boundaries to understand model behavior

## Dataset
The dataset contains airline travel records with flight schedule, route, airline, and pricing information.

### Dataset Columns

| Column | Description |
|---|---|
| `date` | Flight travel date |
| `airline` | Airline name |
| `ch_code` | Airline character code |
| `num_code` | Airline numeric code |
| `dep_time` | Flight departure time |
| `from` | Origin city |
| `time_taken` | Flight duration |
| `stop` | Stop type, such as non-stop or one-stop |
| `arr_time` | Flight arrival time |
| `Destination` | Destination city |
| `price` | Flight ticket price |

## Machine Learning Tasks

### Task 1: Flight Price Classification
The first task focuses on classifying flight price patterns using selected numerical features such as `num_code` and `price`.

This task helps identify how SVM models separate flight records based on airline code and pricing behavior.

### Task 2: Flight Destination Classification
The second task focuses on predicting flight destination categories using selected flight-related features such as `num_code` and `price`.

This task demonstrates how the same dataset can be used for a different classification objective by changing the target variable.

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Support Vector Machine
- LinearSVC
- Jupyter Notebook

## Model Results

The SVM models produced the following accuracy scores for the flight classification analysis:

Model / Kernel	Accuracy
SVC	82.00%
LinearSVC	80.00%
RBF Kernel	82.67%
Polynomial Kernel	81.33%

## Result Interpretation

The RBF kernel achieved the highest accuracy at approximately 82.67%, showing that nonlinear classification performed slightly better than the linear models. This suggests that the relationship between selected flight features and the target class may not be perfectly linear.

The LinearSVC model also performed reasonably well, but the nonlinear RBF model provided a better separation between classes.

## Conclusion

This project demonstrates how Support Vector Machine models can be applied to airline flight data for multiple classification tasks. By comparing linear and nonlinear SVM kernels, the analysis showed that the RBF kernel performed best with an accuracy of approximately 82.67%. The project also highlights how decision boundary visualizations can help explain model behavior and compare classification approaches.

Overall, this project is a strong machine learning portfolio example because it uses one real-world-style dataset for two related classification objectives: flight price classification and flight destination prediction.
