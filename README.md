# 🎧 Podcast Listener Engagement Prediction with PySpark & XGBoost

## 📌 Project Overview

This project predicts podcast listener engagement by analyzing features such as episode length, guest popularity, content sentiment, and publishing patterns to estimate listening time (in minutes). It leverages the scalability of **PySpark** and the performance of **XGBoost** to build efficient and interpretable models on large datasets.

## 📊 Data Features

The dataset contains various attributes categorized as follows:

- **Content Features**: Episode duration, genre, episode number, sentiment analysis
- **Publication Patterns**: Day and time of publication
- **Social Elements**: Host popularity, guest presence and popularity
- **Monetization Factors**: Number of advertisements

## 🛠️ Technical Implementation

### Data Processing Pipeline
- **Missing Values**: Genre-specific median imputation for missing episode lengths
- **Feature Engineering**:
  - Binary indicator for guest presence
  - Extraction of numeric episode numbers from titles
  - Categorical encoding of publication time and sentiment
  - Frequency scoring for podcast popularity

### Machine Learning Architecture
- **Framework**: Distributed XGBoost integrated with PySpark
- **Training**: 3-fold cross-validation with parallel execution
- **Tuning**: Grid search on tree depth, learning rate, and number of estimators
- **Evaluation Metric**: Root Mean Square Error (RMSE)

### Cloud Integration
- **Data Storage**: AWS S3 for scalable and distributed data access
- **Development Environment**: Databricks notebooks for collaborative ML workflows

## 📈 Model Performance

- **Validation RMSE**: 13.05  
Demonstrates strong predictive performance on listener engagement.

## 💻 Technologies Used

- **PySpark**: Scalable data processing and ML pipelines
- **XGBoost**: Efficient gradient boosting implementation
- **AWS S3**: Cloud-based data storage
- **Databricks**: Development and execution environment

## 🔍 Key Insights

The project helps podcast creators:

- Identify content characteristics that drive higher engagement
- Optimize publishing schedules for better reach
- Balance monetization strategies with listener retention (ads vs. satisfaction)

## 🚀 Future Enhancements

- Analyze feature importance to understand the top drivers of engagement
- Incorporate time series modeling to capture seasonal listening trends
- Develop an A/B testing framework to test content hypotheses
- Integrate engagement predictions into recommendation systems

## 📚 Skills Demonstrated

- Large-scale data processing using PySpark
- Distributed machine learning with XGBoost
- End-to-end feature engineering and data preparation
- Cloud service integration (AWS S3)
- Hyperparameter tuning and performance evaluation
- Cross-validation for model reliability
