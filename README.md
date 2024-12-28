# Reveal-Categories-Found-in-Data
App publishers want to know what users think and feel about their apps. While it's impossible to read their minds, you can data-mine the reviews they leave to uncover the main topics. This project utilizes clustering and Natural Language Processing (NLP) techniques to analyze negative reviews from the Google Play Store, sort them into categories, and identify key terms from each category.
## Project Overview
In this project, the objective was to analyze the negative reviews of a mobile app from the Google Play Store. By applying clustering and Natural Language Processing (NLP) techniques, the project aimed to sort these reviews into meaningful categories. This helps app publishers understand common themes and pain points expressed by users, allowing them to prioritize improvements and address concerns effectively.

By using K-means clustering and TF-IDF vectorization, this analysis uncovered the most prominent topics in the negative reviews, providing insights into the areas of the app that users find unsatisfactory. The main categories of the reviews were identified based on the content of the text, helping to break down the negative feedback into digestible, actionable insights.
## Tools and Libraries
- Pandas: For handling and processing the review data.
- NumPy: For numerical operations and handling arrays.
- NLTK (Natural Language Toolkit): For tokenization, stopword removal, and text preprocessing.
- Scikit-learn: For machine learning and clustering algorithms (K-means) and text vectorization (TF-IDF).
- Reviews Data: A dataset containing a sample of reviews and their respective scores (from 1 to 5) in the Google Play Store, provided as a CSV file (reviews.csv).
## Key Tasks
1. Preprocessing Negative Reviews:
- Filter reviews with scores of 1 or 2, identifying them as negative.
- Tokenize the reviews and remove stop words and non-alphabetic characters.
- Store the preprocessed reviews in a pandas DataFrame for further analysis.
2. TF-IDF Vectorization:
- Use the TF-IDF (Term Frequency-Inverse Document Frequency) method to convert the preprocessed reviews into numerical vectors.
- This vectorization helps capture the importance of each word in the context of the entire corpus of reviews.
3. K-Means Clustering:
- Apply K-means clustering to group the reviews into 5 categories.
- Analyze the clusters and label each review with its respective cluster category.
4. Identifying Key Terms for Each Cluster:
- For each cluster, identify the most frequent term by summing the TF-IDF scores across all reviews within that cluster.
- Store these terms, along with their frequency, in a new DataFrame that represents the key topics of the negative reviews.
5. Analysis & Reporting:
- Output a DataFrame containing the most frequent term and its associated category for each cluster.
- Provide insights into the main issues faced by users based on the identified clusters.
