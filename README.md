# Tutorials prepared for the ["Summer School: Machine Learning in Quantum Physics and Chemistry"](https://ml2021.ckc.uw.edu.pl/)

**DISCLAIMER:** The majority of the code prepared within tutorials comes from our great lecturers, i.e., *Eliska Greplova*, *Roman Krems*, *Giuseppe Carleo*, *Filippo Vicentini*, *Florian Marquardt*, and their collaborators (see the list of authors in the beginning of every notebook). Moreover, Borja Requena Pozo with Gorka Muñoz Gil prepared the notebook on reinforcement learning. I (Anna Dawid) am responsible only for gathering these materials in one place and adapting to meet the needs of participants of our school (i.e., adding comments, solutions, information on using Google Colaboratory, hyperparameters, comparing Tensorflow and PyTorch, etc.).

## Hands-on Tutorial A: Phase Classification with Unsupervised and Supervised Machine Learning (by Eliska Greplova)
Folder "A - Phase Classification (by Eliska Greplova)" contains:
- a folder `Ising_data` with Monte-Carlo generated configurations of Ising spins on a 30x30 lattice with labels as well as configurations of spins from Ising Gauge Theory (IGT) with labels. In particular:
  - `ising_training_configs_30x30.npy` contains configurations of Ising spins belonging to the training set,
  - `ising_training_labels_30x30.npy` contains labels, i.e., temperatures of Monte Carlo samples of Ising spins belonging to the training set,
  - `ising_test_configs_30x30.npy` contains configurations of Ising spins belonging to the test set,
  - `ising_test_labels_30x30.npy` contains labels, i.e., temperatures of Monte Carlo samples of Ising spins belonging to the test set,
  - `ilgt_training_configs.npy` contains configurations of IGT spins belonging to the training set,
  - `ilgt_training_labels.npy` contains labels, i.e., temperatures of Monte Carlo samples of IGT spins belonging to the training set,
  - `ilgt_test_configs.npy` contains configurations of IGT spins belonging to the test set,
  - `ilgt_test_labels.npy` contains labels, i.e., temperatures of Monte Carlo samples of IGT spins belonging to the test set.

The folder also contains:
- a Jupyter notebook `01_Unsupervised_learning.ipynb` which aims at clustering states from both models into corresponding phases with Principal Component Analysis (PCA) and t-Stochastic Neighborhood Embedding (t-SNE),
- a Jupyter notebook `02_Supervised_learning.ipynb` where we train neural networks to recognise phases in both models and stress the importance of regularization of ML models,
- a Jupyter notebook `03_More_sophisticated_NN_methods.ipynb` where we implement ["learning by confusion"](https://www.nature.com/articles/nphys4037) and ["predictive model"](https://iopscience.iop.org/article/10.1088/1367-2630/ab7771/meta) to detect phase transition in the Ising model.

## Hands-on Tutorial B: Gaussian Process Regression (by Roman Krems)
Folder "B - Gaussian Process Regression (by Roman Krems)" contains:
- a file `H3O+.csv` with 6D potential energy surface (PES) for the molecule $H_3O^+$ (with six first columns listing the coordinates and the seventh - the energy),
- a Jupyter notebook `Gaussian_process_regression.ipynb` with the exemplary code to build Gaussian process (GP) regression of 1D synthetic data with simple kernels, and three tasks:
  1. To extend the code to do GP regression of the 6D PES of $H_3O^+$.
  2. To use four different kernels (provided by sklearn).
  3. To build more complex kernels using the Bayesian Infomation Criterion (BIC) as model selection metric (as described in lectures).
Solutions of the tasks were prepared by Anna Dawid, are only exemplary, and have no ambitions of being the optimal solutions.

## Hands-on Tutorial C: Neural-Network Quantum States (by Filippo Vicentini and Giuseppe Carleo)
Folder "C - Neural-Network States (by Giuseppe Carleo)" contains:
- a Jupyter notebook `00_Introduction_to_JAX.ipynb` which is an introductory notebook about Jax, talking a bit about everything and terminating with an example of a linear regression (a useful addition that was not covered during the school in Warsaw).
- a Jupyter notebook `01_Introduction_to_NetKet.ipynb` which introduces the syntax of ["NetKet 3"](https://www.netket.org/), a very useful library for studies of many-body quantum systems with neural networks and ML techniques, on the example of the Ising model,
- a Jupyter notebook `02_Dynamics_with_NetKet.ipynb` which was the basis of ["Filippo Vicentini's lecture"](https://youtu.be/Ryz-o71tuy8).
All notebooks were prepared by Filippo Vicentini and accompanied the lectures of Giuseppe Carleo.

## Hands-on Tutorial D: Reinforcement Learning (by Florian Marquardt)
Folder "D - Reinforcement Learning (by Florian Marquardt)" contains:
- a Jupyter notebook `Reinforcement_learning.ipynb` which introduces the concepts of Q-table, deel Q-learning, and policy gradient. It was prepared by Borja Requena Pozo and Gorka Muñoz Gil to illustrate the lectures of Florian Marquardt.