# Facebook Engagement Analysis

**Predicting Post Engagement Using Linear Regression**

This project analyzes a Facebook page dataset to understand the factors that drive post engagement. Using Python, data exploration, feature engineering, and machine learning, I built regression models to predict how much interaction a post will receive.

The goal of this project is to demonstrate a full data science workflow, from raw data exploration to predictive modeling.

## Project Overview

Social media engagement is an important metric for businesses and creators. Understanding what factors influence engagement can help optimize content strategy.

In this project, I analyzed a dataset of Facebook posts to answer the following question:

| ***What factors influence the number of interactions a Facebook post receives?***

The project focuses on predicting Total Interactions, which represents the total number of likes, comments, and shares.

## Key Questions

The analysis focused on identifying factors that influence engagement:  
	1.	Does paid promotion increase engagement?  
	2.	Do timing variables such as month, weekday, or hour affect interactions?  
	3.	Does post reach or impressions correlate with higher engagement?  
	4.	Can we build a machine learning model that predicts post interactions?  

## Repository Structure
```
facebook-engagement-analysis
│
├── data
│   ├── raw
│   │   └── dataset_Facebook.csv
│   └── cleaned
│       └── facebook_cleaned.csv
│
├── code
│   ├── 01_explore.ipynb
│   ├── 02_transform.ipynb
│   └── 03_model.ipynb
│
├── docs
│   └── images
│
└── README.md
```

## Dataset

Dataset: **Facebook Metrics Dataset**

This dataset contains information about posts published on a Facebook page, including:  
	•	Post type  
	•	Posting time  
	•	Paid promotion status  
	•	Reach and impressions  
	•	Engagement metrics  

## Target Variable

**Total Interactions**

```Total Interactions = Likes + Comments + Shares```

This value represents the total engagement a post receives.

## Project Workflow

The project follows a typical data science pipeline.

## 01. Exploratory Data Analysis (EDA)

Notebook: 01_explore.ipynb

During this phase, the dataset was explored to understand patterns and detect potential issues.

Key steps included:  
	•	Inspecting dataset structure  
	•	Identifying missing values  
	•	Exploring feature distributions  
	•	Visualizing relationships between variables  
	•	Detecting outliers using boxplots  
	•	Evaluating correlations between variables  

EDA helped identify features that may influence engagement and prepared the dataset for modeling.

## 02. Data Cleaning & Preprocessing

Notebook: 02_clean.ipynb

Data preparation steps included:

**Handling Missing Values**  
Some columns contained missing values that needed to be addressed before modeling.

**Encoding Categorical Variables**  
Categorical variables such as post type were converted into numerical form.

**Feature Selection**  
Features directly related to the target variable (e.g., likes, comments, shares) were removed to prevent data leakage.

**Log Transformation**  
The target variable Total Interactions was log-transformed to reduce skewness and improve model performance.

**Feature Scaling**  
Numerical features were scaled to ensure fair contribution during model training.

The cleaned dataset was then saved for use in modeling.

## 03. Model Development

Notebook: 03_model.ipynb

Several regression models were tested to predict post engagement.

**Linear Regression**  
A baseline linear regression model was created to predict engagement.

**Ridge Regression**  
Ridge regression was used to reduce overfitting by applying L2 regularization.

**Lasso Regression**  
Lasso regression was tested to perform feature selection through L1 regularization.

These models help determine how different features contribute to predicting engagement.

## Model Evaluation

Model performance was evaluated using:  
	•	R² Score  
	•	Mean Squared Error (MSE)  
	•	Train vs Test comparison   

These metrics helped measure how well the models generalized to unseen data.

## Key Insights

Some important findings from the analysis include:  
	•	Post reach and impressions strongly correlate with engagement  
	•	Paid posts may increase visibility but do not always guarantee higher engagement   
	•	Certain posting times appear to perform better  
	•	Log transformation improved model stability by reducing extreme skew  

These insights highlight how visibility and timing can impact social media performance.

## Technologies Used

	•	Python  
	•	Pandas  
	•	NumPy  
	•	Matplotlib  
	•	Seaborn  
	•	Scikit-learn  
	•	Jupyter Notebook  

## Future Improvements

This project could be expanded by:  
	•	Performing hyperparameter tuning  
	•	Using advanced models (Random Forest, Gradient Boosting)  
	•	Performing cross-validation  
	•	Building a dashboard to visualize engagement insights  
	•	Analyzing content features such as captions or hashtags  

## Author

Nick Peril

Aspiring Cloud & Data Professional with experience in:  
	•	Python  
	•	Data analysis  
	•	SQL  
	•	AWS cloud technologies  

Currently building projects that combine data analytics and cloud computing.

 If you found this project interesting, feel free to explore the notebooks and reach out!