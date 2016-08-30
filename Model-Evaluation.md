Model Evaluation
================

V 3
---

Final metrics


|Model                      | Rank 1 score | test score | timeit     |
| ------------------------- |:------------:|:----------:|:----------:|
| Random Forests            | -1.008       | 0.94800    | 4943.46 s  |
| Logistic Regression       | -1.020       | 1.01616    | 41.07 s    |
| Naive Bayes               | -1.068       | 1.06087    | 0.59 s     |
| Decision Tree             | -0.954       | 0.95053    | 518.45 s   |
| KNN                       | -1.537       | 1.45483    | 169.49 s   |
| ExtraTreesClassifier      | -1.023       | 1.02850    | 3924.89 s  |
| AdaBoost                  | -1.045       | 1.03726    | 1276.17 s  |
| GradientTreeBoosting      | -0.945       | 0.93574    | 9553.61 s  |


The metric used for model evaluation is [log loss][logLoss].
V 2
---
After this [post](data_leak) that talked about the data leakage in the model, I will be 
using features that can be obtained when an animal is first brought to shelter. Hwnce I will
no longer be using age of the animal, as the dataset actually contains age of the animal on 
outcome. However I shall be continuing to use the gender and also the fact that they are 
spayed/neutered. Reason being that most animal shelters and ASPCA in particular allows 
requests to neuter/spay an intact animal once if they want. Also there are many animals 
that reach the shelter already spayed/neutered. 

V 1
---
Uses barebones features, no tuning of any parameters for any algorithms.
Features used:

1. Age
2. Gender - Neutered male, spayed female, intact male/female
3. has a name
4. Cat/Dog

I have not taken breed, color and time of outcome.

|Model                      | CV score1   | CV score2   | CV score3   | test score | timeit   |
| ------------------------- |:-----------:|:-----------:|:-----------:|:----------:|:--------:|
| Random Forests            | -1.16617897 | -1.2112944  | -1.11520838 | 1.12426    | 3.24 s   |
| Logistic Regression       | -0.97484274 | -0.96763943 | -0.9647996  | 0.96547    | 464 ms   |
| Naive Bayes               | -1.22157213 | -1.26583667 | -1.20188548 | 1.21500    | 4.49 ms  |
| Decision Tree             | -1.38918722 | -1.45546753 | -1.34826891 | 1.24844    | 13 ms    |
| SVM                       | -0.94089612 | -0.94775816 | -0.92365895 | 0.93214    | 1min 36s |
| KNN                       | -4.76794659 | -4.08102411 | -5.56083471 | 4.42387    | 73.4 ms  |
| ExtraTreesClassifier      | -1.37822642 | -1.42679228 | -1.33020657 | 1.22868    | 88 ms    |
| AdaBoost                  | -1.55363168 | -1.55128592 | -1.55373471 | 1.55451    | 789 ms   |
| GradientTreeBoosting      | -0.85764033 | -0.85404969 | -0.84077597 | 0.84521    | 464 ms   |
| *Bag Logistic Regression  | -1.04228698 | -1.03388775 | -1.02656614 | 1.03262    | 840 ms   |
| *Bag SVC                  | -8.1003993  | -8.14571116 | -7.73783385 | 7.79678    | 26.5 s   |
| *Bag Decision Tree        | -0.94326021 | -0.9617784  | -0.93770676 | 0.95734    | 47.9 ms  |
| *Bag KNN                  | -0.94996338 | -0.9414747  | -0.96176933 | 0.95716    | 343 ms   |
| *Bag Naive Bayes          | -0.94672725 | -0.94512211 | -0.9854242  | 0.94647    | 54.2 ms  |



[logLoss]: https://www.kaggle.com/wiki/LogarithmicLoss


