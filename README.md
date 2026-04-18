This project analyzes a dataset of Udemy courses to uncover the key factors that drive course success and builds a machine learning model to predict the number of subscribers.

Objectives
Identify what makes a course successful on Udemy
Perform data cleaning and exploratory data analysis (EDA)
Build a machine learning model to predict course popularity
Extract meaningful business insights from the data

Tools & Technologies
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn (Machine Learning)

Dataset Features
Course title, subject, and level
Price and free/paid status
Number of subscribers and reviews
Course duration and number of lectures
Published date

Data Cleaning

Key preprocessing steps included:

Converted price from string (e.g., "$50", "Free") to numeric
Standardized content_duration by converting minutes into hours
Extracted year and month from published timestamps
Handled missing values by removing invalid rows

Exploratory Data Analysis (EDA)
Key Findings from Correlation Analysis
Strong positive correlation (0.65) between:
num_reviews and num_subscribers
Strong relationship (0.80) between:
num_lectures and content_duration
Weak correlation between price and subscribers

Feature Importance (Model Insights)

The most important features influencing course popularity:

Number of Reviews (~0.72) → strongest predictor
Number of Lectures (~0.10)
Price (~0.08)
Content Duration (~0.06)
Level and subject have minimal impact

Key Insights
Courses with more reviews tend to attract significantly more subscribers
Course length (lectures + duration) positively impacts engagement
Price has a relatively small effect on subscriber count
Beginner-friendly courses dominate the platform
External factors likely play a role beyond dataset features

Project Outcome

This project demonstrates how raw data can be transformed into actionable insights and predictive models using data science techniques.

Future Improvements
Use advanced models (XGBoost, Gradient Boosting)
Perform hyperparameter tuning
Add text analysis on course titles
Build a recommendation system