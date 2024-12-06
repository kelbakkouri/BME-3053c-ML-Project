You can find various graphs on how the ML model has interprested and predicted the data. Note that the various graphs give information on accuracy and feature importance, as well as time to train model and performance while training. 

The first code blocks go one part at a time. 
Block one just imports needed packages
Block two will import the data set from openml datasets. We included the appropiate data set into the github in case you do not have access to openml.
Block three will preprocess data to effectively work in the ML model. 
Block four is for creating a training set and a testing set. 
Block five sets up the classification report and provides recall, f1-scores, precision, and displays a text confusion matrix. Accuracy should be around 85% 
Block six creates a graphical representation of the confusion matrix and an ROC (receiver operating characteristic). The better the model the higher the area below the curve is. Our specific tests had around .91 out of 1. 
Block seven uses an SVM model rather than a logistic regression model. -84%
Block eight uses a Random Forest model. -94%
Block 9 saves the model
Block 10 will redo the ROC curve with any of the previous model created. 
Block 11 will run the Feature importance. This will show us how important each parameter is to predicting whether someone has heart disease. 
Block 12 runs a Precision-Recall Curve which shows how well the model does with recall vs. precision. 
Block 13 runs all the previous graphs in one run
Block 14 is for creating a gui to predict heart disease with the 11 given statistics. 

Dependencies include:
ipywidgets
pandas
numpy
scikit-learn
matplotlib
tkinter may also be used if desired for creating the GUI.
