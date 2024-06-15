# Author-Age-Detection-System
**Used Methods:**

### Data Preparation and Preprocessing:
1. **Cleaning Text Data**: 
   - Removal of non-alphanumeric characters, digits, and extra spaces.
   - Conversion of text to lowercase.
   - Removal of stopwords using a list of French stopwords from NLTK.
   - Lemmatization of words to reduce them to their base or root form.

2. **Feature Extraction**:
   - **TF-IDF Vectorization**: Text data was transformed into a TF-IDF matrix, which helps to evaluate how important a word is to a document in a collection of documents.

### Machine Learning Models:
1. **Logistic Regression**: Utilized with hyperparameter tuning through grid search to optimize 'C', 'penalty', and 'solver'.
2. **Support Vector Machine (SVM)**: Implemented with different kernels ('linear', 'rbf') and regularization parameter tuning.
3. **Multinomial Naive Bayes**: Applied with a focus on adjusting the 'alpha' parameter and whether to fit prior probabilities or not.

### Deep Learning Models:
1. **Custom Neural Network Architecture**:
   - A sequence model using TensorFlow and Keras, comprising embedding layers, LSTM layers, dense layers, and dropout for regularization.
   - Compiled with binary crossentropy loss and Adam optimizer, trained to classify text into two age groups.
2. **BERT for Sequence Classification**:
   - Utilization of BERT (Bidirectional Encoder Representations from Transformers) tokenizer and model specifically for sequence classification tasks.

### Deployment:
- **FastAPI** for creating a web API to deploy the model, allowing users to make predictions by submitting text through a simple web interface.

These methods are indicative of a comprehensive approach to handling text data, leveraging both traditional machine learning and advanced deep learning techniques to classify text based on the age group of the author.
