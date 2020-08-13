# Data-Challenge-for-Fitbod-Yunge-Li

This project include two sections, EDA and modeling as time series forecasting.
The raw data is raw workout recordings. In order to process in-depth exploration and straightforward visualization,
some feature engineering and creation work is included in the EDA section (part 3. Preliminary Data Exploration).

The general framework is as below.

For the EDA part:
  1. Raw Data Loading
    1.1 Data Type Conversion ('Date': string -> datetime.datetime)
    1.2 Measuring Unit Conversion ('Weight': kg -> lb)
    
  2. Data Ingestion
    2.1 Feature Classification based on Data Type
    2.2 Data Missing and Imputing (Space & NaN)
    2.3 Data Duplication and De-duplication
    2.4 Outliers and Elimination for Each Feature (Univariate Distribution and Visualization)
      2.4.1 Date
      2.4.2 ExerciseId and ExerciseName
      2.4.3 Reps and Weight
      2.4.4 User
      
   3. Preliminary Data Exploration
    3.1 User Engagement and Workout Frequency
      3.1.1 Historical Engagement for Each User
      3.1.2 Registration Time Span for Each User
      3.1.3 Times of Workout in the Recent 7 Days
      3.1.4 Times of Workout in the Recent 30 Days
      3.1.5 Times of Workout in the Recent 3 Months(90 Days)
      3.1.6 Times of Workout in the Recent 1 Year(365 Days)
      3.1.7 Times of Workout in 7 days after the First Workout
      3.1.8 Times of Workout in 30 days after the First Workout   
      3.1.9 Times of Workout in 90 days after the First Workout
      3.1.10 Most Recent Workout
      3.1.11 Decriptive Statistics based on the Newly Created User Engagement Table
      3.1.12 Feature Distribution
      3.1.13 Churn Rate Visualization (fit Beta Distribution)
      3.1.14 Inter-Feature Correlation using Pearson Corr
     
     3.2 Users' Preference on Exercise
      3.2.1 Popularity of Exercises
      3.2.2 Exercise pattern in the first 7 days after registration
        - Popularity of Exercises 
        - Reps distribution for each exercises
        - Weights distribution for each exercises
        - Number of sets per workout for each exercises
        - Number of sets completed by each user for each exercises
        - Correlation between Different Exercises using Pearson Corr
      3.2.3 Exercise pattern for users in 7-30 days after registration
        - Popularity of Exercises 
        - Reps distribution for each exercises
        - Weights distribution for each exercises
        - Number of sets per workout for each exercises
        - Number of sets completed by each user for each exercises
        - Correlation between Different Exercises using Pearson Corr
      3.2.4 Overall Reps/Weights Distribution for Each Exercise
      
      3.3 DAU Fluctuation
        3.3.1 Dist on the whole time window
        3.3.2 Dist on each year
        3.3.3 Dist on holidays
        3.3.4 Correlation between holiday and DAU using Kendall-Tau Corr
        3.3.5 Diff in engagement between holiday users and not-holiday users
        
  4. Data Modeling —— Time Series Forecasting on Active Users
      4.1 Preliminary Analysis and Visualization
      4.2 Resampling
      4.3 Implement Baseline Time-Series Prediction Model using Prophet with Dafault Hyperparameter Settings
      4.4 Model Tuning and Optimization
        4.4.1 Changepoints Exploration
        4.4.2 Holiday Impact Analysis
       
        
      
         
      
      
      
   
