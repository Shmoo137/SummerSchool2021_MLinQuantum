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

For similar excercises but in PyTorch instead of Tensorflow, see ["Eliska's course at TU Delft"](https://www.eliskagreplova.com/ai-for-physicists-ap3751).