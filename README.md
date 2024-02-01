# Housing Prices ML 

### Project Overview

Data science analysis leveraging machine learning algorithms (Linear Regression & Random Forest) to gather
insights on factors such as population and income, with the target variable being median housing price in CA.

This project involved extensive data preprocessing and model optimization to enhance predictive accuracy and
provide a comprehensive understanding of the complex relationships influencing housing prices.

### Data Sources

Housing data (primary dataset): https://www.kaggle.com/datasets/camnugent/california-housing-prices

### Tools

- Excel
- Jupyter Notebooks
- Python

### Results/ Findings

#### Correlations: 
- Strong positive correlations were observed between total number of rooms (total_rooms), total bedrooms (total_bedrooms), population, and households.
- A negative correlation of -0.49 was found between 'INLAND' (a categorical variable indicating whether a house is inland or not) and 'median_house_value'. Houses near the ocean tended to have higher prices compared to inland properties.
- Multicollinearity issues were acknowledged due to the strong interrelatedness of features, and it was mentioned that further analysis and modeling techniques might be needed to address these issues.
- 
#### Visualizations: 
- A scatterplot was suggested to visualize the relationship between coastal proximity and property values.

#### Linear Regression Model: 
- The linear regression model was used to predict housing prices based on the given features.
- Standard scaling was applied to the training data using StandardScaler.
- Logarithmic transformations were applied to certain features in the test data, such as 'total_rooms', 'total_bedrooms', 'population', and 'households'.
- Dummy variables were created for the 'ocean_proximity' categorical feature.
- Additional features, 'bedroom_ratio' and 'household_rooms', were created in the test data.
- The linear regression model was trained using the scaled training data.
- The model's performance was evaluated on the test data, and the output score was reported as 0.6779274051870232.

The output score of 0.6779 indicates the coefficient of determination, commonly known as R-squared. It measures the proportion of the variance in the dependent variable ('median_house_value') that is predictable from the independent variables in the model. An R-squared of 0.6779 suggests that approximately 67.79% of the variance in the housing prices can be explained by the features included in the linear regression model. This value ranges from 0 to 1, with higher values indicating a better fit of the model to the data. In this case, the model shows a relatively good fit, but further analysis and refinement may still be considered based on domain knowledge and the specific goals of the analysis.

