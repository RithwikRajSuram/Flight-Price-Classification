# Flight Price Classification using Support Vector Machine Kernels

## Project Overview
This project analyzes airline flight price data using Support Vector Machine classification models. The goal is to classify flight price patterns using flight-related features such as airline code numbers and ticket price, then compare different SVM kernel performances.

## Dataset
The dataset contains airline travel records with the following columns:

- date
- airline
- ch_code
- num_code
- dep_time
- from
- time_taken
- stop
- arr_time
- Destination
- price

## Tools and Libraries Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

## Analysis Performed
- Loaded and explored airline flight price data
- Selected numerical features for model training
- Used airline code numbers and price as model inputs
- Trained Support Vector Machine models with different kernels
- Compared model accuracy across SVM kernels
- Visualized decision boundaries for sigmoid, linear SVC, and RBF kernels

## Model Results
The SVM models produced the following accuracy scores:

| Model / Kernel | Accuracy |
|---|---:|
| SVC | 82.0% |
| Linear SVC | 80.0% |
| RBF Kernel | 82.67% |
| Polynomial Kernel | 81.33% |

## Key Visualization

### SVM Kernel Decision Boundaries
The decision boundary plot compares how different SVM kernels separate flight price groups using code numbers and price.

- The sigmoid kernel creates a sharper nonlinear split.
- The linear SVC model separates classes using mostly straight boundaries.
- The RBF kernel creates a smoother nonlinear boundary and produced the highest accuracy in this analysis.

## Conclusion
This project demonstrates how Support Vector Machine models can be applied to airline flight price data for classification. Among the tested models, the RBF kernel achieved the highest accuracy at approximately 82.67%, showing that nonlinear classification performed slightly better than the linear and sigmoid approaches.
