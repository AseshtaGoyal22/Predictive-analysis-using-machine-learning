# Predictive-analysis-using-machine-learning

*COMPANY*- CODTECH IT SOLUTION

*NAME*- ASESHTA GOYAL

*INTERN ID*- CT04DA481

*DOMAIN*- DATA ANALYTICS

*DURATION*- 4 WEEKS

*MENTOR*- NEELA SANTOSH

## Project Description: Social Media Post Engagement Classification

In this internship project, I built an end to end machine learning pipeline to classify social media posts as having either high or low engagement, based on various faetures available in the dataset. This task is an essential part of understanding how machine learning models are developed, trained, and evaluated in a real world scenario.

## Tools and Technologies Used:

1. Apache Spark(PySpark): The entire machine learning pipeline was developed using PySpark, the Python API for Apache Spark. PySpark is widely used in big data environments and is particularly useful for working with large datasets due to its distributed processing capabilities.

2. Google Colab: All development and experimentation were conducted in Google Colab, a cloud based Jupyter Notebook environment provided by Google. It offers free access to compute resources, including GPUs, and supports integration with various Python libraries, making it ideal for developing and testing machine learning workflows.

3. Python Libraries:

   - pandas and numpy were used for initial inspection and testing of the dataset before switching to PySpark for the complete model pipeline.
  
   - PySpark modules like StringIndexer, OneHotEncoder, VectorAssembler, LogisticRegression, and BinaryClassificationEvaluator were used to prepare data, train the model, and evaluate its performance.

## Problem Statement and Objective:

The main objective of this project was to build a classification model that predicts whether a social media post is likely to receive high enagagement. Engagement, in this context, refers to user interactions like likes and comments. To achieve this, I defined a binary label:

- 1-> high engagement(if likes are greater than or equal to the median number of likes),
- 0-> low engagement(if likes are below the median).

The dataset included several faetures such as:

- post_type: the type of content posted(e.g., image, video, text)
- likes: the number of likes the post received
- comments: number of comments
- device_type: device used to post(e.g., mobile, desktop)
- location: geographical location of the user

The target variable (engagement_label) was derived by calculating the median of the likes column.

## Model Development and Evaluation:

1. Feature Engineering: Categorical features such as post_type, device_type, and location were encoded using StringIndexer followed by OneHotEncoder. Numerical features like comments were used directly. All features were then assembled into a single feature vector using VectorAssembler.

2. Model Training: A Logistic Regression model was trained on 80% of the data, while the remaining 20% was used for evaluation. Logistic Regression was chosen due to its simplicity and effectiveness in binary classification problems.

3. Model Evaluation: The model was evaluated using ROC-AUC (Receiver Operating Characteristic- Area Under Curve). This metric helps to understand how well the model distinguishes between high and low engagement posts.

## Real World Applications:

This project has numerous real world applications across social media, digital marketing, and content recommendation systems. For example:

- Content Strategy: Platforms like Instagram, Facebook, or LinkedIn can use such models to recommend optimal content types to users for better engagement.

- Ad Targeting: Brands can priortize content that is more likely to perform well, helping to increase ROI on advertisements.

- User Engagement Analytics: This kind of analysis helps product teams improve the design and functionality of their apps to encourage more user interaction.

- Spam Detection or Boosting Quality Content: Posts with consistently low enagagement may be deprioritized or flagged, while high engagement content can be boosted.

## Conclusion

This project has helped me gain hands on experience with PySpark, machine learning workflows, feature engineering, and model evaluation. It also gave me practical exposure to working with real world data, making decisions about target variable creation, and applying classification algorithms to predict outcomes. These skills are foundational for a career in data science and machine learning, and this task has been a valuable step in my professional journey.
