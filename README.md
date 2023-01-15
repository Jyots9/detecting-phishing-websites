# detecting-phishing-websites
OBJECTIVE
The goal of this research is to train deep neural networks and machine learning models using the dataset produced to identify phishing websites. The necessary URL- and website content-based attributes are retrieved from the dataset formed by the collection of both phishing and benign URLs of websites. Every model's performance is measured and contrasted.

DATASET COLLECTION
 https://www.unb.ca/cic/datasets/url-2016.html. This dataset has a collection of benign, spam, phishing, malware & defacement URLs. Out of all these types, the benign and phishing url dataset are considered for this project. From this dataset, 1500 random legitimate and phishing URLs (each) are collected to train the ML models.
 
 FEATURE EXTRACTION
 The following feature categories were taken from the URL data:
    1.Address Bar based Features
          In this category 9 features are extracted.
    2.Domain based Features
          In this category 4 features are extracted.
    3.HTML & Javascript based Features
          In this category 4 features are extracted.
  All together 17 features are extracted from the 3000 URL dataset and are stored in 'final_data.csv' file.
  The features are referenced from the https://archive.ics.uci.edu/ml/datasets/Phishing+Websites.
  
  MODELS & TRAINING
 This data set comes under classification problem, as the input URL is classified as phishing (1) or legitimate (0). The supervised machine learning models (classification) considered to train the dataset in this project are:

Decision Tree
Random Forest
Multilayer Perceptrons
XGBoost
KNeighbors Classifier
Support Vector Machines
Extra Trees Classifier

HYPERPARAMETER TUNING
The top three models with the highest accuracy were selected, and the Grid Search was used to fine-tune their parameters.
ENSEMBLE Technique
Objective here is to make more stable model,than focussing on the accuracy. Voting is used where these 3 models in final are merged

RESULTS
From the obtained results of the above models, XGBoost Classifier has desirable model performance. So the model is saved to the file 'XGBoostClassifier.pickle.dat'
  
