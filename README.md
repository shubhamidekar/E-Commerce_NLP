# Text Classification NLP Project

This repository contains a Jupyter Notebook showcasing a text classification project aimed at categorizing text into predefined categories using Natural Language Processing (NLP) techniques. The project employs two models for classification: Multinomial Naive Bayes and Convolutional Neural Network (CNN), with a focus on preprocessing, text vectorization, and model evaluation.

## Preprocessing Steps

The preprocessing pipeline consists of several steps to clean and prepare the text data for modeling:

1. **Expand Contractions**: Convert shortened words to their full forms (e.g., "isn't" to "is not").
2. **Remove Punctuations**: Eliminate all punctuation symbols from the text.
3. **Tokenization**: Break down text into individual words or tokens.
4. **Convert to Lower Case**: Normalize the text by converting all characters to lower case.
5. **Remove Words Containing Numerical Digits**: Filter out any words that contain numbers.
6. **Remove Stopwords**: Eliminate common words that carry minimal useful information.
7. **Stemming/Lemmatization**: Reduce words to their root form or base dictionary form.

## Text Vectorization

Text vectorization is a critical step in transforming textual data into numerical vectors so that machine learning algorithms can understand and process the text. This project uses techniques suitable for the models employed, preparing the data for the classification task.

## Model Evaluations

### Multinomial Naive Bayes Model

- **Accuracy**: ~94%
- **Precision**, **Recall**, and **F1-Score** across categories like Books, Clothing & Accessories, Electronics, and Household range between 0.90 to 0.98, indicating strong performance in correctly classifying instances.
- **Macro Avg**: 0.94
- **Weighted Avg**: 0.94

### CNN Model

- **Overall Accuracy**: ~97%
- **Precision**, **Recall**, and **F1-Score** for each category are high, ranging from 0.97 to 0.98, suggesting excellent balance and accuracy in predictions.
- **Macro Avg and Weighted Avg** similarly reflect high performance.

## Interpretation

Both models demonstrate robust performance, with the CNN model slightly outperforming the Multinomial Naive Bayes model in terms of overall accuracy and balance between precision and recall. The preprocessing steps and text vectorization techniques play a crucial role in achieving high model performance.

## How to Use

1. Clone this repository to your local machine.
2. Ensure you have Jupyter Notebook installed, or use [Google Colab](https://colab.research.google.com/) for an online alternative.
3. Open the `TextClassification.ipynb` notebook and replace the 'eCommerceDataset.csv' with this Kaggle dataset 'https://www.kaggle.com/datasets/saurabhshahane/ecommerce-text-classification' download it on your local machine before
4. Run the cells sequentially to observe the preprocessing, model training, and evaluation steps.

## Requirements

- Python
- Jupyter Notebook
- Scikit-learn
- NLTK and Poter Stemmer library
- TensorFlow/Keras for CNN model

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
