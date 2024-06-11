# Black Friday Sales Prediction

![Black Friday Sales Prediction](https://searchengineland.com/figz/wp-content/seloads/2014/12/black-friday1-ss-1920.jpg)

## Table of Contents
- [Project Introduction](#project-introduction)
- [Dataset Description](#dataset-description)
- [EDA](#eda)
- [Data Preparation](#data-preparation)
- [Modeling Phase](#modeling-phase)
- [Evaluation Metric](#evaluation-metric)
- [Conclusion](#conclusion)

### Project Introduction
Black Friday, the Friday following Thanksgiving Day in the United States, marks the beginning of the Christmas shopping season. It has been a significant shopping day since 1952, although the term "Black Friday" became widely used more recently. Retail stores and eCommerce businesses face the challenge of setting product prices to maximize profit during these sales. This project aims to predict product prices based on historical sales data, helping stores optimize pricing strategies for maximum profit.

### Dataset Description
The dataset, sourced from an Analytics Vidhya hackathon, includes features such as age, gender, marital status, product categories, city demographics, and purchase amounts. It contains 12 columns and 537,577 records. Our goal is to predict the purchase amount for each product.

### EDA
Key insights from the exploratory data analysis (EDA) include:
- Approximately 75% of purchases are made by male users, indicating that males are the primary contributors to sales.
- Single men spend the most during Black Friday, while spending tends to decrease after marriage.
- Consumers aged 25-40 are the highest spenders.
- People who have lived in a city for 1 year tend to spend more, possibly because they are still settling in and buying new items.
- City B contributes the most to overall sales income, but City C is significant for specific product sales.

### Data Preparation
- **Label Encoding**: Applied LabelEncoder to categorical columns like Age, Gender, and City_Category.
- **Dummy Variables**: Used `get_dummies` from Pandas for the Stay_In_Current_City_Years column.
- **Missing Values**: Filled missing values in Product_Category_2 and Product_Category_3.

### Modeling Phase
- Split the dataset into an 80:20 train-test ratio.
- Implemented several supervised models, including Linear Regressor, Decision Tree Regressor, and Random Forest Regressor.

### Evaluation Metric
The model's performance was evaluated using Root Mean Square Error (RMSE), which measures the average squared differences between predicted and actual values. Lower RMSE values indicate better model performance.

### Conclusion
We implemented multiple supervised models such as Linear Regressor, Decision Tree Regressor, Random Forest Regressor, and XGBoost Regressor. Among these, the XGBoost Regressor achieved the best performance with an RMSE score of 2879, indicating its superior predictive capability for this dataset.

By using this predictive model, retail stores can better forecast product sales and adjust prices strategically to maximize profits during Black Friday sales.
