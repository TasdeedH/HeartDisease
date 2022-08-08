# NeuralNetworks

A comprehensive paper produced pertaining to predictive capabilities of two supervised learning models (The Multilayer Perceptron and The Support Vector Machine)

Programming Languages: Python (Numpy, Pandas, Matplotlib, Seaborn, Imblearn and PyTorch)

This paper constructs, assesses and critically compares two supervised learning approaches in determining whether a patient is likely to develop Coronary Heart Disease (CHD) within the next 10 years.

Before beginning to perform a data analytics project in this domain, it was imperative to develop a working domain expertise so that data could be effectively cleaned in the context of the domain, and so that conclusions found could be corroborated. This was done through an extensive literature review, some of which can be found in the final report. Examples of analysis included, before modelling, included outlier analysis, missing value analysis (some of which led to imputations using MICE) as well as feature engineering.

Since this was a realistic dataset, there was naturally a heavy imbalance in the class proportions to those not expected to develop CHD to those who are (85:15) - therefore suitable strategies needed to be developed to accomodate this when modelling. This was done through a combination of oversampling (SMOTE-NC to accomodate for categorical features) and undersampling (Edited Nearest Neighbours) which were all integrated into a pipeline consisting of cross validation and hyperparameter tuning as a means to prevent data leakage.

Multiple variants for each model were considered in which the optimal variant for each model were then compared, in terms of various domain-specific metrics, time taken to fit and predict, AUC scores and various visualisations such as ROC curves, using mathematical,computational and domain knowledge to hypothesize and explain reasoning for results. Results from the report show large improvements in modelling performance with out proposed pipeline compared to not accounting for the imbalance at all.

Further lines of enquiry were identified as well as highlighting reasons for the development of such models within the heart health domain, broadly citing references.

NC_Report_FINAL.pdf provides the full report highlighting the motivation for the problem, insight into the models of choice, EDA, methodology, hypotheses, critical evalutation of results and further study
MainProcessing.ipynb provides a detailed exploratory data analysis and data cleaning/processing of the heart disease dataset
MainModelling.ipynb provides a detailed view of the thought processing regarding the modelling as well as its execution
BestMLP.ipynb and BestMLP.ipynb are the Jupyter Notebook scripts for the optimal variants of each model
