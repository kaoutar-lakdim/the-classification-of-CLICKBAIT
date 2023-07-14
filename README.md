# CLICKBAIT Classification - Implementation of Machine Learning Approaches


<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/c585d9a1-85e1-405c-86d4-cdc256586230" alt="schema">
</p>


In the scope of our project, we focused on the classification of article titles as clickbait or non-clickbait by applying various machine learning algorithms. This project will result in a report and an oral presentation.

Beyond learning to work collaboratively as a group, the objective was to expand our scientific and technological knowledge. As we discovered, machine learning combines computer science and mathematics. For our team, it was a complete exploration of text data preprocessing techniques.

Our initial goal was to discover and understand these techniques to proceed with their implementation and apply different learning algorithms to the processed data. The ultimate objective of our project was to compare these learning algorithms and create the best classification model.



## Table of Contents

- [Text Classification](#text-classification)
- [The Proposed Model for Clickbait Classification](#the-proposed-model-for-clickbait-classification)
- [Text Preprocessing Techniques](#text-preprocessing-techniques)
- [EDA: Exploratory Data Analysis](#eda-exploratory-data-analysis)
- [Feature Extraction](#feature-extraction)
- [Training Different Classification Models](#training-different-classification-models)
- [Comparison of Classification Models](#comparison-of-classification-models)
- [Conclusion](#conclusion)

## text-classification

Text classification is a machine learning technique that assigns a predefined set of categories to open text. Text classifiers can be used to organize, structure, and categorize almost any type of text, ranging from documents and medical studies to files and the web.

For example, news articles can be organized by topics, support tickets can be organized by urgency, chat conversations can be organized by language, brand mentions can be organized by sentiment, and so on. Text classification is one of the fundamental tasks in natural language processing with extensive applications such as sentiment analysis, topic labeling, spam detection, and intent detection.

## the-proposed-model-for-clickbait-classification
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/5f3d60ca-f3ee-4add-830b-622da9b11d0d" alt="schema">
</p>

## Text Preprocessing Techniques

Text preprocessing is a method used to clean textual data and prepare it for inputting into a model. Textual data contains noise in various forms, such as emotions, punctuation, and text in different cases.

When we discuss human language, there are multiple ways to express the same thing, and this poses the main challenge we must confront because machines do not understand words. They require numerical representations, so we need to convert the text

<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/139a485d-38c1-4977-b487-7c4ae3251e0f)" alt="schema">
</p>

## EDA: Exploratory Data Analysis
###  World Cloud :
Before running the models, we analyzed the word frequencies of clickbait titles and non-clickbait titles. There were clear distinctions in the vocabulary as well as overlaps, as shown in the WordClouds below.
A WordCloud is a visual representation of words where the size of each word corresponds to its frequency or importance.
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/c53872b6-0742-4b77-acd4-261dcc9f1435" alt="schema">
</p>

#### Word Cloud of Clickbait Titles
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/c53872b6-0742-4b77-acd4-261dcc9f1435" alt="schema">
</p>

#### Word Cloud of Non-Clickbait Titles
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/31550f8e-0f10-446f-ac83-46c7b313537f" alt="schema">
</p>

### Building a word frequency dictionary

In our objective of clickbait title classification, we have defined a dictionary in which we can search how many times a word appears in clickbait or non-clickbait titles. This will be very useful during the feature extraction from the dataset
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/a6395d52-e10c-49c7-be7b-c229cec495c2" alt="schema">
</p>

This graph is easy to interpret. It shows that words like "dinner" and "mani" are clickbait words, while the word "dropout," for example, is a normal word



## Feature Extraction
We have added three columns to our dataframe: bias, bait, and normal.
bait: indicates the number of occurrences of a word in clickbait titles
normal: indicates the number of occurrences of a word in non-clickbait titles
bias: a bias with a value of 1 for all titles

#### The dataframe becomes:
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/c72bd487-6441-4f1f-9ef0-244f5a6fd3d4" alt="schema">
</p>

## Training Different Classification Models

We train several commonly used classification models, such as Naive Bayes classifiers, Support Vector Machines (SVMs), and neural networks. We detail the training, evaluation, and optimization steps for each model.

We have divided our dataset as follows:

Train set: 80%
Test set: 20%

## Comparison of Classification Models

In this part, we compare the performance of different classification models using metrics such as accuracy, recall, and F1-score. We discuss the advantages and disadvantages of each approach and identify the best model for clickbait title classification.

### Without cross-validation
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/a502078e-0ede-4ea6-a107-da69aac6dfa5" alt="schema">
</p>

### With cross-validation
<p align="center">
  <img src="https://github.com/kaoutar-lakdim/the-classification-of-CLICKBAIT/assets/74473164/ab1e5e69-c57f-44bb-84dc-f4c1229b8716" alt="schema">
</p>

We can see that the results obtained with cross-validation are better.

## Conclusion

In conclusion, this project highlights the effectiveness of machine learning approaches for clickbait title classification. We have explored different text preprocessing techniques, extracted relevant features, and trained multiple classification models. The results demonstrate the importance of choosing the right approach to address the clickbait classification problem.


