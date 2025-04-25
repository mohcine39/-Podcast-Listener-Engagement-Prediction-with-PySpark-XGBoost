🎧 Podcast Listener Engagement Prediction with PySpark & XGBoost
🔍 Project Summary
This project leverages PySpark and XGBoost within a big data environment to predict how long users engage with podcast episodes. By processing large-scale datasets, we identify key factors influencing listener behavior and provide insights to optimize content, publication strategy, and monetization.

📁 Data Overview
The dataset includes various features related to podcast content and its context of publication:

Content Attributes: Episode duration, genre, episode number, sentiment score

Publishing Patterns: Day of the week, time of release

Social Signals: Host popularity, guest presence, guest influence

Monetization: Ad count per episode

🛠️ Data Engineering & Pipeline
Missing Data Handling: Imputed missing episode durations using genre-specific medians

Feature Engineering:

Binary indicators for guest presence

Extraction of numerical values from episode titles

Categorical encoding (e.g., day/time/sentiment)

Frequency-based popularity scoring

🤖 Model Architecture
Framework: Distributed XGBoost using PySpark MLlib

Training Process:

3-fold cross-validation

Grid search over learning rate, tree depth, and number of estimators

Evaluation: RMSE (Root Mean Square Error)

☁️ Cloud & Platform
AWS S3: Scalable storage and access to training data

Databricks: Notebook-based development and parallel model training

📈 Model Results
Achieved a validation RMSE of 13.05, indicating strong model performance in predicting listener engagement across varied podcast profiles.

💡 Business & Strategic Insights
This model helps podcast teams to:

Identify content elements that drive engagement

Optimize release schedules for maximum impact

Align guest and ad strategies for better retention and revenue

🚀 Potential Improvements
Feature importance analysis to highlight key engagement drivers

Incorporate time series trends (e.g., seasonal effects)

Add A/B testing frameworks for content variation experiments

Extend to real-time recommendation system integration

🧠 Key Skills Demonstrated
Big Data Processing with PySpark

Distributed Machine Learning with XGBoost

Feature Engineering & Data Transformation

Cloud Integration (AWS S3)

Model Tuning & Evaluation

Cross-Validation at Scale
