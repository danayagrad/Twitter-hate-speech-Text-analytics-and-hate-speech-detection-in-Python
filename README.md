# Twitter-hate-speech-Text-analytics-and-hate-speech-detection-in-Python

Hate speech detection model were built from Crowdflower Twitter hate speech dataset.  5 models were builts from numbers of each English characters, number of each Part of Speech, number of special character and message property extracted from each tweet, 70 attributes in total.


1. Summary: 
	1. Text processing: cleaning noise, irrelevant text such as html code, and removing stopwords. 
	    Used bs4, re.sub, nltk.corpus and nltk.tokenize packages for this step.
	2. Feature extraction: convert text data into numerical data which are numbers of apperance of English character, Part of Speech, special characters, and text properties in each tweet.
	3. Data cleaning: remove outlier and missing value, change data type, normalize data, split training and testing set with stratify sampling method.
	4. Models building and tuning: total of 5 models with grid search tuning and manual tuning for neural network. 5 fold cross validatoin used for tuning and selecting best configuration for each model.
	5. Prediction: Confusions matrix, accuracy, precision and recall were calculated using sklearn.metrics package

2. Tool: 
	- Python for data cleaning and model building. 
	- Posit(Weir. , G. R. S., 2009. Corpus profiling with the posit tools. Liverpool, s.n.) for text features extraction.


3. Algorithms: Random Forest, Linear Regression, SVM, Naive Bayes, and Nueral Network models.

4. Evaluation: Confusions matrix, accuracy, precision and recall.

5. Dataset: The dataset contains 14,513 tweets which were categorised by the judgement of 3 contributors. Each tweet was assigned to one of these classes - contained hate speech, was offensive but without hate speech, or was not offensive. The dataset is credited to Thomas Davidson, Dana Warmsley, Michael Macy, and Ingmar Weber. 2017. "Automated Hate Speech Detection and the Problem of Offensive Language" at the 11th International Conference on Web and Social Media (ICWSM).
