# Invariance-Based-Adversarial-Training

- This Project analyzes the behaviour of a CNN when it is trained with Invariance-Based Adversarial Examples. It is part of my bachelorthesis.
- Throughout the whole experiment the MNIST-Dataset is used.
- The behaivor is analyted on a Vanilla Model and a pre-trained Model with Perturbation-Based Adversarial Examples.
- The Algorithm to generate Invariance-Based Adversarial Examples is from https://github.com/ftramer/Excessive-Invariance

### Results

- The labels for Invariance-Based Adversarial Examples must be determined by humans
- Retraining a model that is pretrained with Perturbation-Based Adversarial Examples with Invariance-Based Adversarial Examples doesn't have a positive impact
- The only helpful solution to gain robustness agains Perturbation-Based Adversarial Examples and Invariance-Based Adversarial Examples is to train a Vanilla Model simultanously with both kinds of Adversarial Examples

## Prerequisites

Make sure you have installed all of the following prerequisites:

- [Tensorflow](https://www.tensorflow.org)
- [Foolbox](https://foolbox.readthedocs.io/en/stable/)
- [Numpy](https://numpy.org/)
- [Keras](https://keras.io/)
- [Matplotlib](https://matplotlib.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)
- [Scipy](https://scipy.org/)

Install all necessary dependencies using pip:

```bash
pip install tensorflow
pip install keras
pip install foolbox
pip install matplotlib
pip install numpy
pip install sklearn
pip install scipy
```

## Explanation of the structure

- The folder "data" contains all data necessary for the code to run
- The folder "data/invarianca-Examples_tramer" contains the Invariance-BAsed Adversarial Exampels provided by Tramer et al. https://github.com/ftramer/Excessive-Invariance
- The folder "models" contains all models necessary for the code to run
- The file "creation_and_triaining.ipynb" creates the necessary CNNs, trains them and conducts all experiments
- The file "evaluation.ipynb" evaluates the results of the experiments
- The file "util.ipynb" only contains utility functions necessary for my bachelorthesis to create images
