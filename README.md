# Machine-Learning-UPM
Assignments for the Machine Learning subject (UPM's Computational Biology Master)

## Supervised:

Developing machine learning models to predict the treatment response of cancer patients, given 21 genetic features (SNPs).

Binary classification problem, the following models were employed: logistic regression, decision tree, KNN, random forest, and multilayer perceptron. In all cases, a basic grid search hyperparameter tuning was performed. Logistic regression and decision trees were interpreted.

Improvements I would make if I did this project today:
- SNPs have two alleles, AB is phenotipically the same as BA. In the problem, I would consider 'WM' and 'MW' to be the same class.
- A more efficient hyperparameter tuning could be performed using Bayesian optimization (for example with the Ax library, see my [optimization repository](https://github.com/javierlopezrodriguez/optimization)).
- Because it is a very small dataset, if I had the computational power, I would evaluate the models using nested cross validation (using cross validation twice, once on the trainval-test division, and a second time on the train-val division), which would give a more unbiased estimate of the generalization error.

## Unsupervised:

Unsupervised machine learning to explore and gain information about a cancer cell line dataset (60 cell lines, expression values of 9994 genes).

Performed hierarchical clustering and partitional clustering, evaluating the different procedures and interpreting the different results.

Improvements I would make if I did this project today:
- Using more methods, sklearn has a wide variety of unsupervised machine learning algorithms that we could try.
- Trying unsupervised deep learning methods, such as autoencoders. The analysis of the latent space of a (variational) autoencoder could provide additonal meaningful information.
