Model Evaluation
================

The metric used for model evaluation is [log loss][logLoss].

V 1
---
Uses barebones features, no tuning of any parameters for any algorithms.
Features used:

1. Age
2. Gender - Neutered male, spayed female, intact male/female
3. has a name
4. Cat/Dog

I have not taken breed, color and time of outcome.

|Model                 | CV score1   | CV score2   | CV score3   | test score | timeit   |
| -------------------- |:-----------:|:-----------:|:-----------:|:----------:|:--------:|
| Random Forests       | -1.16617897 | -1.2112944  | -1.11520838 | 1.12426    | 3.24 s   |
| Logistic Regression  | -0.97484274 | -0.96763943 | -0.9647996  | 0.96547    | 464 ms   |
| Naive Bayes          | -1.22157213 | -1.26583667 | -1.20188548 | 1.21500    | 4.49 ms  |
| Decision Tree        | -1.38918722 | -1.45546753 | -1.34826891 | 1.24844    | 13 ms    |
| SVM                  | -0.94089612 | -0.94775816 | -0.92365895 | 0.93214    | 1min 36s |
| KNN                  | -4.76794659 | -4.08102411 | -5.56083471 | 4.42387    | 73.4 ms  |
| ExtraTreesClassifier | -1.37822642 | -1.42679228 | -1.33020657 | 1.22868    | 88 ms    |
| AdaBoost             | -1.55363168 | -1.55128592 | -1.55373471 | 1.55451    | 789 ms   |


[logLoss]: https://www.kaggle.com/wiki/LogarithmicLoss


