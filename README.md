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
- This code base is made for demonstrating the relation among climate change indecies and gender inequality factors.
We used GDP per capita, Poverty index, Education participation rate from World Bank and Temperature Rise data from Global Data Lab and Nasa.

### Data Collection 
- [GDP per capita](https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?locations=1W).
- [Poverty GINI index](https://data.worldbank.org/indicator/SI.POV.GINI).
- [Education Participation](https://data.worldbank.org/indicator/SE.PRM.CUAT.MA.ZS?end=2023&start=2023&view=bar).
- [Temp-Global datalab](https://globaldatalab.org/geos/download/surfacetempyear/?levels=1&interpolation=0&extrapolation=0).
- [Temp-Nasa](https://data.giss.nasa.gov/gistemp/graphs/graph_data/Global_Mean_Estimates_based_on_Land_and_Ocean_Data/graph.txt).


### Data Preprocessing
- Filled values with mean.
- Only taken common countries of all data 136 countries.
- 

### Exploratory Data Analysis
- Tried different ML models Support Vector Machine, KNN, Ensamble Learning, Random Forest, Linear regression.
- Found Random Forest model more accurately Education Participation Rate. 

### Analysis
- Detailed analysis of the relationship between gender inequality and climate change.

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

