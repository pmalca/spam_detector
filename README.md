# Spam Text Message Classification

This repository contains a Python script for classifying text messages as spam or non-spam. The script utilizes the sklearn library for feature extraction and classification, and the NLTK library for text preprocessing.

## Project Overview

The Spam Text Message Classification script performs the following steps:

1. **Importing the Libraries**: The necessary libraries, including pandas, sklearn, and nltk, are imported to support the text classification task.

2. **Loading the Datasets**: The script loads the spam text message dataset from Kaggle and encodes the text for further processing.

3. **Cleaning the Dataset**: A text cleaning function is defined to lowercase the text, remove special characters and punctuation, remove stopwords, and join the remaining tokens back into text.

4. **Feature Extraction**: The script uses the TF-IDF technique to convert the text into numerical features. TF-IDF calculates the importance of each word in a document based on its frequency in the document and its rarity across all documents.

5. **Training the Classification Model**: The script uses Logistic Regression, a supervised machine learning algorithm, to train a classification model. Logistic Regression uses the numerical features obtained from TF-IDF to predict whether a text message is spam or non-spam.

6. **Model Evaluation**: The trained model is used to predict the labels for the testing data. The accuracy of the model is calculated and a classification report is generated, which includes precision, recall, and F1-score for both spam and non-spam classes.

7. **Findings**: The results of the model indicate high accuracy, precision, and recall in classifying non-spam messages. Although the recall for spam messages is relatively lower, the model still achieves a reasonable F1-score, suggesting its ability to identify a significant portion of spam messages.

8. **Confusion Matrix**: A confusion matrix is generated to provide a detailed view of the model's performance, showing the counts of true positive, true negative, false positive, and false negative predictions.

## Getting Started

To use the Spam Text Message Classification script, follow these steps:

1. Clone this repository to your local machine.

2. Ensure you have the required dependencies installed by running `pip install -r requirements.txt`.

3. Update the file path in the script to point to your own dataset file if you have a different dataset to classify.

4. Run the script using `python spam_text_classification.py`.

5. The script will output the accuracy, classification report, and confusion matrix for the classification model.

## Contributing

Contributions to this project are welcome! If you have any suggestions, bug fixes, or enhancements, feel free to submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE). You are free to modify and use the code as per the license terms.

## Acknowledgments

Special thanks to the team at Kaggle for providing the spam text message dataset, and to the developers of the sklearn and NLTK libraries for their contributions to the open-source community.

