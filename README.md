# SpamHam Detection Project

Spam detection is a critical process in identifying and flagging unsolicited or unwanted messages, commonly sent in bulk through various communication channels such as emails, text messages, or comments on social media posts. The primary goal of spam detection is to prevent these messages from reaching the intended recipient's inbox, as they can be annoying, time-consuming, and potentially dangerous. Spam can include phishing emails, malware, or scams that attempt to steal personal information or trick the recipient into taking harmful actions.

## Purpose

The purpose of this project is to classify messages as either spam or ham (non-spam). By accurately categorizing messages, we aim to enhance cybersecurity measures and ensure that users receive only relevant and safe content.

## Dataset Description

The "Spam-Ham SMS" dataset is a well-known labeled dataset used for spam classification tasks. It consists of 5,572 SMS messages, with 4,827 messages labeled as "ham" (non-spam) and 747 messages labeled as "spam." Although the exact recording year is unspecified, the dataset was compiled and made publicly available by researchers at the University of California, Irvine (UCI) in 2012.

## Data Fields

- **v1:** Indicates if the SMS message is ham or spam. "Ham" means it is not spam.
- **v2:** The SMS message itself.

## Labels

- **Spam:** Erroneous messages that need to be detected.
- **Ham:** Messages that are not spam, labeled as ham.

## Cleaning the Raw Data

Data preprocessing is crucial for building an effective machine learning model. The following steps were applied to clean the raw data:

- **Lowercasing:** Convert all text to lowercase.
- **Special Character Removal:** Delete characters that do not add value to the meaning of the text.
- **Stopword Removal:** Eliminate common words that do not carry much information.
- **Hyperlink Removal:** Delete hyperlinks that may not contribute to the classification.
- **Number Removal:** Remove numerical values.

Additionally, stemming and lemmatization techniques were used to reduce words to their root form, optimizing the model's accuracy.

## Tokenization

Tokenization, the process of splitting text into smaller chunks or tokens, was employed. Each token serves as an input feature for the machine learning algorithm.

## Word Embedding

Word embedding techniques, specifically word2vec and Continuous Bag of Words (CBOW), were utilized to represent words in a numerical form, enhancing the model's ability to understand semantic relationships.

## Data Balancing

Both undersampling and oversampling techniques, including Synthetic Minority Over-sampling Technique (SMOTE), were applied to address class imbalances and improve the model's generalization.

## Models Used

The following machine learning models were employed for classification:

- **Decision Tree Classifier**
- **K-Nearest Neighbors (KNN)**
- **Support Vector Classification (SVC)**

These models were chosen for their effectiveness in text classification tasks.

This project aims to contribute to the field of spam detection, providing insights into the efficiency of different models and techniques in classifying messages accurately.
