Readme
======
[![license]https://img.shields.io/badge/license-MIT%20License-blue.svg](https://opensource.org/licenses/MIT)
This repository contains my attempts at learning various techniques and methods
to solve a ML classification problem. The problem chosen is a competition from [Kaggle][kaggle],
the [Shelter Animal Outcomes][comp]. 

The tools used are the excellent [scikit learn][sklearn], [jupyter][jupyter], [matplotlib][matplotlib], [seaborn][sns]
and [pandas][pandas].

The problem is to predict the probabilities of an animal getting adopted, transfered, death from 
natural causes, euthanasia, or returned to it's owner. The following features are given to us
age, breed, color, gender, spayed/neutered/intact, whether it's a cat/dog, has a name, etc.

The suggested reading order would be:

1. [Visualization][visualization]
2. [Data cleaning][cleaning]
3. [Random forests][rndmForest]
4. [Logistic Regression][logisticRegression]
5. [Naive Bayes][naiveBayes]
6. [Decision Tree][decisionTree]
7. [SVM][svm]
8. [KNN][knn]
9. [ExtraTreesClassifier][etc]
10. [AdaBoost][adaBoost]
11. [GradientTreeBoosting][gradientBoost]

You can look at the model evaluations [here][modEval]

[Kaggle]: https://www.kaggle.com
[comp]: https://www.kaggle.com/c/shelter-animal-outcomes
[sklearn]: http://scikit-learn.org/
[jupyter]: http://jupyter.org/
[matplotlib]: http://matplotlib.org/
[sns]: https://web.stanford.edu/~mwaskom/software/seaborn/
[pandas]: http://pandas.pydata.org/

[visualization]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-Visualization.ipynb
[cleaning]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-dataCleaning.ipynb
[rndmForest]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-Random-Forests.ipynb
[logisticRegression]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-Logistic-Regression.ipynb
[naiveBayes]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-Naive-Bayes.ipynb
[decisionTree]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-Decision-Tree.ipynb
[svm]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-SVM.ipynb
[knn]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-KNN.ipynb
[etc]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-ExtraTreesClassifier.ipynb
[adaBoost]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-AdaBoost.ipynb
[gradientBoost]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/notebook/shelterAnimalOutcomes-GradientTreeBoosting.ipynb

[modEval]: https://github.com/krispingal/shelterAnimalOutcomes/blob/master/Model-Evaluation.md
