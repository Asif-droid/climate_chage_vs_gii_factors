# Gender Inequality and Climate Change Analysis

This Jupyter Notebook, `gender_inequality_climate.ipynb`, explores the relationship between gender inequality and climate change. The analysis leverages various data visualization and data manipulation libraries in Python to provide insights into how these two critical issues intersect.

## Prerequisites

Ensure you have the following Python libraries installed:

- `numpy`
- `matplotlib`
- `pandas`
- `sklearn`
- `tpot`
- `tensorflow`

You can install these libraries using pip:

```bash
pip install numpy matplotlib pandas sklearn tpot tensorflow
```
## Contents

### Introduction
- This project visualizes the impact of temperature rise on education participation rates and explores how temperature, GDP, and poverty rates can predict changes in education participation using various machine learning models. It utilizes models such as Support Vector Machines (SVM), K-Nearest Neighbors (KNN), Ensemble Learning, Linear Regression, and Random Forest for predictive analysis. The repository contains data preprocessing, visualization, and model implementation to understand the relationships between these factors and how climate change may influence education outcomes.

### Data Collection 
- [GDP per capita](https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?locations=1W).
- [Poverty GINI index](https://data.worldbank.org/indicator/SI.POV.GINI).
- [Education Participation](https://data.worldbank.org/indicator/SE.PRM.CUAT.MA.ZS?end=2023&start=2023&view=bar).
- [Temp-Global datalab](https://globaldatalab.org/geos/download/surfacetempyear/?levels=1&interpolation=0&extrapolation=0).
- [Temp-Nasa](https://data.giss.nasa.gov/gistemp/graphs/graph_data/Global_Mean_Estimates_based_on_Land_and_Ocean_Data/graph.txt).


## Data Preprocessing
Before applying machine learning models, the dataset undergoes the following preprocessing steps to ensure data quality and consistency:

### 1. Duplicate Removal  
Duplicate entries are identified and removed to avoid redundant data points that could skew the model's performance.
### 2. Handling Missing Values (NaN)
Any missing values in the dataset are imputed using the mean value of the respective column to ensure a complete dataset without losing significant information.
### 3. Merging Multiple Data Sources
Data from various sources, including temperature rise, GDP, poverty rate, and education participation rate, are merged to create a unified dataset for analysis. This is done using a common identifier (e.g., `country`, `year`) to align all the variables.
### 4. Feature Scaling (Optional)
If necessary, feature scaling (such as normalization or standardization) is applied to ensure that features like GDP and poverty rate are on the same scale, allowing the models to perform optimally.

## Exploratory Data Analysis
After the data has been preprocessed, the next step is the analysis phase, which involves training various machine learning models to predict education participation rate based on temperature rise, GDP, and poverty rate. The following steps outline the key stages of the analysis process:
### 1. Data Splitting
The merged dataset is divided into two parts: a training set and a test set. The training set is used to train the machine learning models, while the test set is used to evaluate the models' performance.
### 2. Model Selection
Several machine learning models are chosen to predict the education participation rate. The models used include:
- Support Vector Machines (SVM)
- K-Nearest Neighbors (KNN)
- Ensemble Learning (e.g., Bagging, Boosting)
- Linear Regression
- Random Forest
### 3. Training Models
Each model is trained on the training dataset. During training, the models learn to predict the target variable (education participation rate) based on the input features (temperature rise, GDP, and poverty rate).
### 4. Model Evaluation
The performance of each model is evaluated using various metrics such as Mean Absolute Error (MAE) and R-squared (R²). These metrics help in determining the accuracy of the predictions.

## Result Analysis
- Linear Regression
  ```
  Mean Absolute Error (MAE): 19.757518321451506
  Mean Squared Error (MSE): 597.4101825860815
  R-squared (R²): 0.35628188123160587
  ```
- Random Forest
 ```
  Mean Absolute Error (MAE): 3.658859986234793
  Mean Squared Error (MSE): 29.661569266175515
  R-squared (R²): 0.9680392297883378
```
- svm
 ```
  SVR - Mean Squared Error: 16.644423043908322
  SVR - R-squared score: 0.49796212165968234
```
- knn
  ```
  KNN - Mean Squared Error: 14.991569141541337
  KNN - R-squared score: 0.5837427833354114
  ```

- DT
  ```
  Decision Tree - Mean Squared Error: 14.497125053469984
  Decision Tree - R-squared score: 0.6190226501641137
  ```
- Ensamble learning
  ```
  Ensemble (Gradient Boosting) - Mean Squared Error: 12.825334169542966
  Ensemble (Gradient Boosting) - R-squared score: 0.6932644604536435
  ```
- AUTO ML
  ```
  AutoML (TPOT) - Mean Squared Error: 11.01497331125136
  AutoML (TPOT) - R-squared score: 0.7441024580689239
  ```

### Conclusion
- Found Random Forest model more accurately Education Participation Rate than other models.

## Usage

To run the notebook, open it in Jupyter Notebook or JupyterLab:

## Contributing

If you wish to contribute to this project, please fork the repository and create a pull request with your proposed changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any questions or feedback, please contact [Email](asifurbuet98@gmail.com).

