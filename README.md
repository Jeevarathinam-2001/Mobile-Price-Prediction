# Mobile-Price-Prediction

This repository is based on the open source mobile price prediction dataset available in Kaggle
https://www.kaggle.com/datasets/iabhishekofficial/mobile-price-classification

For this problem we need to perform multi-class classification and the number of instances is less than 20k we create and compare linear classifers.
After completing the necessary feature selection and data preprocessing we proceed towards building various ensemble models like Random Forest Classifer, Adaptive Boosting Classifier, XG Boost Classifier.
Among the ensemble models XG Boost performs the best. 
The evaluation metrics used here are accuracy_score, confusion matrix and F1-Score.
Then we build our Support Vector Classifier with both rbf and linear kernels.
We observe that SVC with linear kernel outperforms even the ensemble models.
So now we take Support Vector Classifer as our best model and classify our test data where target is not given.
Finally we pickle our SVC model and save our modified test data in csv file.
