

## Instagram Engagement Analysis

This project analyzes Instagram engagement data to uncover insights about user interactions with posts. The dataset consists of various metrics related to Instagram posts, including impressions from different sources, engagement metrics (likes, comments, shares, saves), and additional contextual information (captions and hashtags).

### Dataset Overview

The dataset includes the following columns:

| Column          | Non-Null Count | Dtype  |
|-----------------|----------------|--------|
| Impressions     | 119            | int64  |
| From Home       | 119            | int64  |
| From Hashtags   | 119            | int64  |
| From Explore    | 119            | int64  |
| From Other      | 119            | int64  |
| Saves           | 119            | int64  |
| Comments        | 119            | int64  |
| Shares          | 119            | int64  |
| Likes           | 119            | int64  |
| Profile Visits  | 119            | int64  |
| Follows         | 119            | int64  |
| Caption         | 119            | object |
| Hashtags        | 119            | object |

### Analysis and Visualizations

1. **Hashtags Used and Their Lengths**:
   - A bar graph illustrating the hashtags used in the posts and their respective lengths.

2. **Distribution of Impressions**:
   - **From Home**: A histogram showing the distribution of impressions coming from the home feed.
   - **From Hashtags**: A histogram showing the distribution of impressions coming from hashtags.
   - **From Explore**: A histogram showing the distribution of impressions coming from the explore section.

3. **Impressions on Instagram Posts From Various Sources**:
   - A pie chart visualizing the proportion of impressions coming from different sources (Home, Hashtags, Explore, Other).

4. **Major Hashtags Used**:
   - Identification of the most frequently used hashtags in the posts.

5. **Relationship Analysis**:
   - **Likes and Impressions**: Scatter plot illustrating the relationship between the number of likes and total impressions.
   - **Comments and Impressions**: Scatter plot illustrating the relationship between the number of comments and total impressions.
   - **Shares and Impressions**: Scatter plot illustrating the relationship between the number of shares and total impressions.
   - **Saves and Impressions**: Scatter plot illustrating the relationship between the number of saves and total impressions.

6. **Heatmap of All Parameters**:
   - A heatmap representing the correlations between all numerical parameters in the dataset.

7. **Profile Visits and Followers Gained**:
   - Analysis of the relationship between profile visits and the number of followers gained.

### Predictive Model

In addition to the above analyses, a predictive model has been created to help users predict the growth of their Instagram profiles based on historical engagement data. This model leverages the various engagement metrics to provide insights into potential future performance.

### Model Evaluation

The performance of several regression models was evaluated to determine the best model for predicting Instagram engagement metrics:

- **Linear Regression**: MSE: 4746059.12, Model Score: 0.878
- **Ridge Regression**: MSE: 4745076.01, Model Score: 0.878
- **Lasso Regression**: MSE: 4745025.67, Model Score: 0.878
- **Random Forest Regressor**: MSE: 4676533.44, Model Score: 0.880
- **Gradient Boosting Regressor**: MSE: 1177156.73, Model Score: 0.970
- **XGBoost**: MSE: 1014109.91, Model Score: 0.974
- **Support Vector Regressor**: MSE: 45587713.52, Model Score: -0.174
- **MLP Regressor**: MSE: 3442022.02, Model Score: 0.911
- **Bayesian Ridge Regression**: MSE: 4039600.12, Model Score: 0.896

**Conclusion**: **XGBoost** and **Gradient Boosting Regressor** are the best models for this dataset, with XGBoost slightly outperforming Gradient Boosting Regressor. These models should be considered for further fine-tuning and potential use in predicting Instagram engagement metrics.

### Usage

The dataset and analysis are intended for educational purposes. It provides a comprehensive overview of Instagram engagement metrics and how they interrelate, helping users understand the dynamics of social media interactions.

### Requirements

- Python 3.x
- pandas
- matplotlib
- seaborn
- scikit-learn
- xgboost

### Conclusion

This project provides valuable insights into Instagram engagement metrics, offering visualizations and analyses that can help users optimize their social media strategies. The predictive model further enhances the utility of this analysis by providing foresight into potential profile growth based on historical data.
