# Sentiment Analysis on Social Media for U.S. Presidential Elections

This project leverages **Apache Spark** to analyze public sentiment expressed in Reddit comments regarding the 2024 U.S. Presidential Election. We developed and evaluated sentiment analysis models using a dataset of tweets from the 2020 U.S. Presidential Election, achieving accuracies of **67.58% (global approach)** and **65% (local approach)**. The model trained with the global approach was subsequently applied to Reddit comments to uncover sentiment trends in 2024 election discussions.

## Key Features
- **Distributed Computing**: Implemented within the Apache Spark environment for scalable data processing.
- **Sentiment Analysis Models**: Developed and tested models trained on the 2020 U.S. Election dataset.
- **High Accuracy**: Models achieved accuracy between **65%-68%**.
- **Scalable Framework**: Evaluated the scalability of the local approach under size-up tests, identifying and addressing limitations due to the SVM algorithm's time complexity.
- **Optimized Data Transfer**: Proposed an intermediate aggregation strategy to reduce data movement during model training under the global approach.

## Results
- Applied the global model to Reddit comments, revealing a balance between **positive and negative sentiments**, both significantly outnumbering neutral sentiments (10%).
- Demonstrated Spark's capability to process large-scale social media data efficiently.

## Technologies Used
- **Apache Spark** for distributed data processing.
- **Support Vector Machines (SVM)** for sentiment classification.
- **Reddit** and **Twitter** datasets for sentiment analysis.

This project highlights the power of distributed computing and advanced machine learning to extract meaningful insights from large-scale social media data. 

The ReadMe file describes the purpose of each notebook:

1. Experimentation Local Approach: Conducts the ensemble effect check, examines the distribution of labels/classes in each partition, and performs the size-up experiment.
   
 2. Prediction: Implements the prediction of sentiments for the processed Reddit comments
   
3. Reddit Comments Preprocessing: Implements the preprocessing of Reddit comments related to the 2024 U.S. Presidential Election

4. SVM Global Approach: Implements the training of a model using the MLlib SVM algorithm (global approach)

5. SVM Local Approach: Implements the training of a model using the traditional scikit-learn SVM algorithm (local approach)

6. Tweets Data Preprocessing and Labeling: Implements the preprocessing and sentiment labeling of the 2020 U.S. Presidential Election Tweets dataset.


