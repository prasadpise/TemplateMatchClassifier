## TemplateMatchClassifier
# Machine Learning in Python - Roll your Own Estimator Example for TemplateMatchClassifier

This notebooks demonstrates how scikit-learn can be extended to include new models by implementing the TemplateMatchClassifier.

The TemplateMatchClassifier is a very basic classification algorithm that calculates the average value of all descriptive features for all instances that have that target level in a training dataset and when asked to make a prediction returns the closet match(based on Euclidean distance) by comparing the descriptive feature values of the query instance to every target level in the template.

The TemplateMatchClassifier is very simple:

Training: For each target feature level calculate the average value of all descriptive features for instances that have that target level. Store these average vectors as templates for each target level.
Prediction: When a new prediction needs to be made compare the descriptive feature values of the new query instance to each template and return the target feature level that belongs to the template that is cloesest (based on Euclidean distance) to the query case.

NOTE THAT THE TEMPLATEMATCHCLASSIFIER IS A TERRIBLE MODEL AND IS ONLY USED AS A VERY SIMPLE DEMONSTRATION OF HOW TO IMPLEMENT AN ML ALGORITHM IN SCIKIT-LEARN
