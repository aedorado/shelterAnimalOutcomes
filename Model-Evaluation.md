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

|Model               | CV score1   | CV score2   | CV score3   | test score |
| ------------------ |:-----------:|:-----------:|:-----------:|:----------:|
| Random Forests     | -1.16617897 | -1.2112944  | -1.11520838 | 1.12426    |
| Logistic Regression| -0.97484274 | -0.96763943 | -0.9647996  | 0.96547    |
| Naive Bayes        | -1.22157213 | -1.26583667 | -1.20188548 | 1.21500    |
| Decision Tree      | -1.38918722 | -1.45546753 | -1.34826891 | 1.24844    |
| SVM                | -0.94089612 | -0.94775816 | -0.92365895 | 0.93214    |


[logLoss]: https://www.kaggle.com/wiki/LogarithmicLoss


