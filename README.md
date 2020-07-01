## Arrhythmia Analysis
In a medical experiment, False Negative is not a desirable outcome. False-negative: A result that appears negative when it should not. An example of a false negative would be if a particular test designed to detect arrhythmia returns a negative result but the person actually does have an arrhythmia. 
This kind of situation can be fatal for the patients, as a false negative diagnosis stop them to refer for further examination. Therefore a correct classification is very much necessary. 

Since this is a supervised classification problem there are a few machine learning algorithm to adapt from such as Decision Tree, Naive Bayes, K Nearest Neighbour and Random Forest etc.

The Naive Bayes approach is based on the idea that the features are conditionally independent and also the features are normally distributed, a quick test shows most of the features are not normally distributed. Keep these in mind we will exclude Naive Bayes as our machine learning algorithm.

K nearest neighbour or KNN another classifier algorithm. The method requires us to develop a similarity or distance on the feature space usually on the basis of a set of predictors or features. Once the distance space is defined, we determine the class by finding the nearest neighbour in the feature space and using that label. Because this model is quite susceptible to noisy data, it is a better idea to find a set of k for k neighbours and then have them vote on the outcome. The value of K has a big impact on the model, if k is small then the classification will be highly impacted by local neighbourhood in contrast, if K is too big then it will respond to most like the response of the population. As a result, normalization is a better choice for KNN as it creates for each variable.

As we know many are better than one and that is the concept of behind the Random Forest algorithm. This is an ensemble learning model that creates multiple decision trees then it aggregates the votes from different decision trees to decide the final class of the test object. The advantages of the Random Forest algorithm are many folds;

 - it is one of the most accurate machines learning algorithm
 - it runs quite efficiently even for very large dataset
 - it can handle quite a complex dataset
 
Although on the downside,

 - Random Forest has the tendency of over-fitting of the model
 - Random Forest is biased in the case of an imbalanced data set.

Because of all these reasons, I will choose the Random Forest as our machine learning algorithm. And We will use Python Scikit-Learn library for that purpose. 
