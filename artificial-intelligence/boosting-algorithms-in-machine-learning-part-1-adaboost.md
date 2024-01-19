# Boosting Algorithms in machine learning, part  1:AdaBoost

In machine learning, boosting is a kind of emsemble learning  method that combines several weak learners into a single strong learner. The idea is to train the weak learners sequentially, each trying to do its best not to repeat the mistakes its predecessor made, eventually building a strong ensemble.

In this article, we will learn one of the popular boosting techniques known as AdaBoost and show how elegantly it allows weak learner to pass on their mistakes to the next weak learner to improve the quality of predictions eventually.

In the opening sentence, I mentioned that boosting is a kind of ensemble learning that combines several weak learners into a single strong learner. Before digging in, we must be familiar with these terminologies first.

## What is an Ensemble?&#x20;

An Ensemble is a technique in mahine where multple models are combined to improve the over performance and generalization of a system. The idea behind ensembling is to leverage the strengths of diferent models and compensate for their individual weaknesses. By combining diverse models, the ensemble can often achieve better results than any of its individual components.

1. Bagging(Bootstrap Aggregating): In bagging, multipleinstances of the same learning algorithm are trained on different subsets of the training data. Each model is trained independently, and their predictions are combined through averaging or voting to make the final prediction. Random Forest is a popular example of a bagging ensemble, where decision trees are trained on different subsets of the data and their predictions are averaged.
2. Boosting: boosting focuses on sequentially training models, with each subsequent model giving more attention to the instances that the previous models found difficult. The predictions of each model are combined in a weighted manner, giving more weight to the models tha perform better. Examples of boosting algorithms include AdaBoost, Gradient Boosting Machines(GBM), and XGBoost.



## Understand why there is a need for boosting algorithms



## Introduction to AdaBoost algorithms



## Implement the AdaBoost algorithm for binary clasification in Python and look at the individual weaklearner as well as the final predictions with some interesting viualizations.

*
