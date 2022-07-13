Seoul Rented Bike Sharing Demand prediction
This markdown only summarize the notebook I made. It does not reflect the whole process. It only aims to answer the question "What has been finally done?" but not how or why.
The objective of this project were to build a support vector machine and decision tree model that could predict rental bike demand. A few kernel functions were also experimented with in the SVM. Decision tree pruning was carried out. Further cross-validation technique was implemented, and the above models were assessed using the dataset. During experimentation, the optimal model is chosen based on performance metrics and learning curves.
Data Preprocessing and Exploratory Data Analysis
Step 1 The date feature is dropped as the prediction performed here is not with repsect to time 
Step 2 Few of the features are renamed for conveience.
Step 3 Checked the null and duplicate values, there are no missing values, null values or duplicate values.
Step 4 Handled the categorical data present in Seasons, Holiday and Functioning Day using OneHotEncoder.
Step 5 Observed the correlation between the features and target variable with the help of heatmap
Step 6 Checked the distrubution of the target variable to choose a threshold for converting it to binary classification form.
Step 7 Dataset is split into train and test set and scaling is done.
Finally the data is normailsed and we have the rented bike demand which needs to be predicted for new observations.

Machine learning models on the dataset 

1. Support Vector Machine(linear, rbf and poly kernel)
2. Decision Tree.(pre and post pruned trees)
Experimented with CV and GridSearchCV 
Plot many learning curves and confusion matrix to fully understand the model's performance.
Comapred different models with the help of performance metrics and ROC -AUC curve.

Concluded that Decision tree with pruning are expected to be more robust for any future addition of training data than SVM.



