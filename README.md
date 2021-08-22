# Tutorials prepared for the ["Summer School: Machine Learning in Quantum Physics and Chemistry"](https://ml2021.ckc.uw.edu.pl/)

**DISCLAIMER:** The majority of the code prepared within tutorials comes from our great lecturers, i.e., *Eliska Greplova*, *Roman Krems*, *Giuseppe Carleo*, *Florian Marquardt*, and their collaborators (see the list of authors in the beginning of every notebook). I (Anna Dawid) am responsible only for gathering them in one place and adapting to meet the needs of participants of our school (i.e., adding comments, information on using Google Colaboratory, etc.).

## Hands-on Tutorial A: Phase Classification with Unsupervised and Supervised Machine Learning (by Eliska Greplova)
Folder "A - Phase Classification (by Eliska Greplova)" contains:
- a folder `Ising_data` with Monte-Carlo generated configurations of Ising spins on a 30x30 lattice with labels as well as configurations of spins from Ising Gauge Theory (IGT) with labels. In particular:
  - `ising_training_configs_30x30.npy` contains configurations of Ising spins belonging to the training set,
  - `ising_training_labels_30x30.npy` contains labels corresponding to phases of Ising spins belonging to the training set,
  - `ising_test_configs_30x30.npy` contains configurations of Ising spins belonging to the test set,
  - `ising_test_labels_30x30.npy` contains labels corresponding to phases of Ising spins belonging to the test set,
  - `ilgt_training_configs.npy` contains configurations of IGT spins belonging to the training set,
  - `ilgt_training_labels.npy` contains labels corresponding to phases of IGT spins belonging to the training set,
  - `ilgt_test_configs.npy` contains configurations of IGT spins belonging to the test set,
  - `ilgt_test_labels.npy` contains labels corresponding to phases of IGT spins belonging to the test set.

After the summer school the folder will also contain:
- a Jupyter notebook `01_Unsupervised_learning.ipynb` which aims at clustering states from both models into corresponding phases with Principal Component Analysis (PCA) and t-Stochastic Neighborhood Embedding (t-SNE),
- a Jupyter notebook `02_Supervised_learning.ipynb` where we train neural networks to recognise phases in both models and stress the importance of regularization of ML models,
- a Jupyter notebook `03_More_sophisticated_NN_methods.ipynb` where we implement ["learning by confusion"](https://www.nature.com/articles/nphys4037) and ["predictive model"](https://iopscience.iop.org/article/10.1088/1367-2630/ab7771/meta) to detect phase transition in the Ising model.

## Hands-on Tutorial B: Gaussian Process Regression (by Roman Krems)
TBA

## Hands-on Tutorial C: Neural-Network States (by Giuseppe Carleo and Filippo Vicentini)
TBA

## Hands-on Tutorial D: Reinforcement Learning (by Florian Marquardt)
TBA