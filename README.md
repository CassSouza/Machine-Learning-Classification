# Machine Learning Classification
Pipeline for classifying samples using different machine learning algorithms, and plots for visualizing and analyzing the results.

## About the data
The __['data.csv'](https://github.com/CassSouza/Machine-Learning-Classification/tree/main/Database)__ dataframe consist of real world data that has been subjected to a clr (centered log-ratio) transformation. Labels and features have had their names changed to generic names in order to preserve the source of the data.

## Machine Learning Algorithms 
Machine learning algorithms available:

+ __[SVM](https://github.com/CassSouza/Machine-Learning-Classification/tree/main/SVM)__ (Support Vector Machine) `SVC classifier`

+ __[ANN](https://github.com/CassSouza/Machine-Learning-Classification/tree/main/ANN)__ (Artificial Neural Network - Multi-layer Perceptron) `MLP classifier`

+ __[RF](https://github.com/CassSouza/Machine-Learning-Classification/tree/main/RF)__ (Random Forest) `RandomForestClassifier`


Inside each folder, there is a .ipynb file with the complete pipeline to build a machine learning model: load the data, build the classification model, and generate the evaluation plots (confusion matrix, Precision-Recall curve, and ROC curve). The evaluation plots can be seen in the .ipynb itself or inside the 'Outputs' folder that are present inside each model folder.  

The parameters of the models were determined through stratified 5-fold cross-validation. Example of the implementtion of this method for the SVM model can be seen in the __[GridSearchCV.ipynb](https://github.com/CassSouza/Machine-Learning-Classification/blob/main/GridSearchCV/GridSearchCV.ipynb)__ file. To adapt the code for other models, it's necessary to adjust the `parameters` variable and the GridSearchCV `estimator` parameter to align with with the chosen model. The search result will then be exported as a .csv file to the __[GridSearchCV](https://github.com/CassSouza/Machine-Learning-Classification/tree/main/GridSearchCV)__ folder.  **Note: GridSearchCV can be computationally expensive, especially when dealing with a large number of hyperparameters, and the process could last several hours.**





