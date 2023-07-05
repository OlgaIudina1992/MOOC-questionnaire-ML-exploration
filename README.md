# MOOC-questionnaire-ML-exploration

The dataset, with thanks: https://www.kaggle.com/datasets/sathyashanmugam/online-edu

# Intro
As the Covid-19 pandemic has clearly shown, the way in which education providers deal with offering online classes impacts not only student performance but also satisfaction. Therefore, collecting and analyzing student feedback is essential to further improve online courses and digital education overall. However, what is the likelihood of a student sharing feedback in the first place? And what are the factors that could allow educators to elicit it?  

To determine the probability of a student volunteering thoughts on the organization and running of a MOOC, data gathered from a number of Indian students attending an online course were wrangled, standardized, put through oversampling to offset scarcity, and plugged into several  machine learning models for testing. Sequential feature selection was later performed on the most successful model to reduce dimensionality and pinpoint the influential parameters.

# Findings
Support vector machine (SVM) algorithm was shown to provide the most reliable results. However, due to the small dataset size and the imbalanced nature of the data, it was unrealistic to expect a very high accuracy from the model. Here are the final metrics:

* Accuracy: 0.6944444444444444
* Precision: 0.7380952380952381
* Recall: 0.7380952380952381
* F1-score: 0.7380952380952381

Confusion matrix:
* TP: 19
* FP: 11
* FN: 11
* TN: 31

* RMSE score: 0.5527707983925667
* Auroc score: 0.6857142857142857
* Log loss: 10.553637170274543

# Final thoughts
Considering all the other scores, this model might be useful in predicting student suggestions with a reasonable error margin.

The most influential parameters for determining whether the student will provide feedback are assumed to be gender, degree program, major,  the platform of study, platform used for student assessment, class frequency and duration.

