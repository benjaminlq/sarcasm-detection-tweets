# <center> Sarcasm Detection in Tweets with Machine Learning and Deep Learning </center>

![](https://img.shields.io/badge/Status-In%20Progress-red)
![](https://img.shields.io/badge/Domain-Natural%20Language%20Processing-blue)
![](https://img.shields.io/badge/Language-Python-green)
![](https://img.shields.io/badge/Package-Scikit--Learn-orange)
![](https://img.shields.io/badge/Package-PyTorch-orange)
![](https://img.shields.io/badge/Package-Hugging%20Face-orange)

## TABLE OF CONTENTS
  - [I. Problem Statement](#i-problem-statement)
  - [II. Dataset](#ii-dataset)
  - [III. Methodology](#iii-methodology)
  - [IV. Results and Discussion](#iv-results-and-discussion)
  - [V. Conclusion](#v-conclusion)
  - [VI. References](#vi-references)

## I. Problem Statement
Sarcasm is the usage of language that normally signifies the opposite to mock or convey contempt. Understanding sarcasm is important as typical sentimental analysis fails to capture the underlying intensions or meanings. In this project, we tackled sarcasm detection on SemEval-2018 (Task 3) English Twitter datasets.

## II. Dataset
The dataset used is English Twitter Dataset provided at SemEval-2018 Task 3 by Van Hee et al. (2018). The dataset consists of 4617 English tweets from 2676 unique users. The tweets are manually labeled using a fine-grained annotation scheme. The dataset consists of a training (3833 tweets) and a testing set (784 tweets) with an 80/20 split ratio.

## III. Methodology
Two main approaches are taken to tackle the binary classification. The first approach uses discriminative classical ML models based on hand-crafted features. The second approach uses deep transformer network to learn the words contextual information using self attention mechanism.

### 1. Classical Models:
#### a/ Architecture
![image](https://user-images.githubusercontent.com/99384454/188254435-ba447b62-0068-4a5c-9232-38b3c5ea2dab.png)

#### b/ Features
Meaningful features: Bisectional contrast of word embeddings, Sentimental maximum contrast inside the tweets. <br>
![image](https://user-images.githubusercontent.com/99384454/188254456-bc7a37d6-8c19-42e8-aa39-8fc9d5c276a9.png)

#### c/ Discriminative Models
![image](https://user-images.githubusercontent.com/99384454/188254533-69b9867e-6e80-4c43-880d-dba051054821.png)

### 2. Transformer Models:
#### a/ Architecture
![image](https://user-images.githubusercontent.com/99384454/188254563-a15e8a75-d17e-455f-8fe0-8900f53f4ef8.png)

#### b/ Models
![image](https://user-images.githubusercontent.com/99384454/188254587-042ec886-45d8-4165-ae44-ee04b6d65725.png)

## IV. Results and Discussion
![image](https://user-images.githubusercontent.com/99384454/188254776-17d87c78-76de-414d-96e3-6d8fc7bf58d7.png)

## V. Conclusion
Several Models were built to tackle Tweeter dataset binary classification problems. In general both classical models and transformer models perform better than the SVM baseline performance. BERT-large model achieved the highest performance on test dataset with F1-Score of **72%**.

## VI. References
- Cynthia Van Hee, Els Lefever, and V´eronique Hoste. 2018a. Semeval-2018 task 3: Irony detection in english tweets. In Proceedings of The 12th International Workshop on Semantic Evaluation, pages 39– 50
