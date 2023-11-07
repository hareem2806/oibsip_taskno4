# oibsip_taskno4
SPAM DETECTION 

Overview: In this dataset the task is to read data from a file containing emails and classify them as 'spam' or 'ham' using a machine learning algorithm.

Importing Libraries: In this section, the necessary Python libraries are imported for the project, including pandas for data manipulation, numpy for numerical operations, and scikit-learn for machine learning tools.

Reading File: This section reads a CSV file named 'spam.csv' and stores it in a Pandas DataFrame called 'df'. The 'ISO-8859-1' encoding is used to read the file.

Exploring DataSet: This part includes several lines of code to explore the dataset. The first few rows, last few rows, shape, column names, summary description, and information about the dataset are displayed, which provides a sense of the data's structure and content.

Handling Data Inconsistencies: This section deals with data inconsistencies, such as missing or null values, dropping unnecessary columns, renaming columns for clarity, and removing duplicate values from the dataset.

Label Encoding: The LabelEncoder from scikit-learn is used to convert text labels in the 'Spam or Ham' column of the DataFrame into numerical values, making it suitable for machine learning.

Splitting the Dataset: The dataset is split into training and testing sets using scikit-learn's train_test_split function. The 'X_train' and 'Y_train' variables hold the training data, and 'X_test' and 'Y_test' hold the testing data.

Text Vectorization: Scikit-learn's TfidfVectorizer is used to transform the email text data into numerical features. The training and testing data are both transformed into TF-IDF vectors.

Model Training: In this part, a Multinomial Naive Bayes classifier is initialized and trained on the transformed training data. The model's accuracy is calculated on the test data.

Model Evaluation: The model's performance is evaluated by making predictions on sample data. Sample texts for both "ham" and "spam" are provided, and the model predicts their labels. Additionally, a confusion matrix and accuracy are displayed for the test data.

Accuracy: The accuracy is of 96.95% . Moreover with sample text the model classifies 3 out of 4 test samples correctly.
