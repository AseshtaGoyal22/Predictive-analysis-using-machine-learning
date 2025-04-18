# Predictive-analysis-using-machine-learning

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

# Model Development and Evaluation:

1. Feature Engineering: Categorical features such as post_type, device_type, and location were encoded using StringIndexer followed by OneHotEncoder.
