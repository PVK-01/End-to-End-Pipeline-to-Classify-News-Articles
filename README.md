# End-to-End-Pipeline-to-Classify-News-Articles
This is a project to classify news articles text to their respective column in which it was published.

## Overview, Aim, and Outcome
The final goal of the project is to classify news articles text into their specific category. The main aim of the project is to get familliar with all the aspect of an end to end projects. This will include: 
- Aeature extraction process
- Dimensionality Reduction Process
- Application of classification models
- Evaluation of the pipeline
- Then using pre trained word embedding techniques like Word2Vec, GLoVE.
- Checking the classification by performing UMAP clustering 


## Data Set
The data set consists of 3150 rows and 8 columns. With the original text of the article present in the column full_text of the CSV file, and the target variable leaf_label contains the data about which news column it was originally written in. This target variable contains 9 classes, where the classes chess, cricket, hockey, soccer, football represent the main label sports, and the classes %22forest%20fire%22, flood, earthquake, drought represent the main label climate. The keywords, summary, and author column contains the main key words, summary and the author of the specific text.

## Feature Extraction
Methods Used:
- Cleaning data from stop words and other non required symbols and text
- Performing lemmatization and count vectorization
- Bag of Words method
- Term Frequency-Inverse Document Frequency Model (TFIDF)

## Dimensionality Reduction
Methods Used:
- Latent Semantic Indexing (LSI)
- Non- negative Matrix Factorization (NMF)

## Application of Simple Classification Models
Methods Used:
- Support Vector Machines (SVM) with hyper parameter tuning
- Logistic regression with no regularization and hyper parameter tuning
- Logistic regression with L1 regularization and hyper parameter tuning
- Logistic regression with L2 regularization and hyper parameter tuning\
- Naive Bayes Classifier
- Naive Bayes Multiclass Classifier
- SVM multiclass one VS Rest method
- SVM multiclass one vs one method
- Dealing with subsampling to deal with class imbalance then again performing multiclass models

## Evaluation the Pipeline
Different dimensionality reduction techniques are compared with eachother and then different classification models are compared with eachother. Then the whole pipeline parameters are compared as a whole using grid search with cross validation.
The metrices used for Evaluation:
- Confusion matrix
- Accuracy
- Precession
- Recall
- F-1 score
- ROC curves

## Replace corpus-level features with pretrained features
Extract word features using a framework called GLoVE: Global Vectors for
Word Representation. A word representation is most often a vector of fixed dimension that captures the meaning of a target word by relating its numerical vector to other vectors in an estimated vector space. GLoVE in particular, measures the similarity between a pair of words by their representations’ Euclidean distance in the vector space of representations.
