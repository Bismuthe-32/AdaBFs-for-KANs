# AdaBFs-for-KANs: Introducing Adaptive Basis Functions for Kolmogorov Arnold Networks

This research explores the use of Adaptive Basis Functions to improve the representational power of Kolmogorov–Arnold Networks (KANs), a function approximation framework inspired by the Kolmogorov–Arnold representation theorem.

Kolmogorov–Arnold Networks approximate multivariate functions by composing sums of univariate functions. In this project, we introduce Adaptive Basis Functions — smooth, learnable components (e.g., radial basis functions or B-splines) — to replace static or hand-designed basis functions typically used in KANs.

Original research paper by Liu et al found [here](https://arxiv.org/pdf/2404.19756)

Official KAN Repo found [here](https://github.com/KindXiaoming/pykan/blob/master/hellokan.ipynb)

# Problem

Adaptive Basis Functions (ABFs) solve the problem of inflexible basis function by introducing learnable parameters. If a true function has irregular non-linear relationships between the variables. Our introduction of Radial Basis Functions built upon the normal distribution dynamically fine-tunes to optimize the center and standard deviation based on the dataset and the true function.

Secondly, fixed basis functions can lead to consistent approximation error, leading to high bias if their form is mismatched to the target function.

# Why Adaptive Basis Functions (ABFs)
ABFs introduce learnable parameters into basis function that allow closer approximation and optimization to represent the true function. Over real-world datasets, variables have complex relationships that cannot be deteted by a regular KAN with fixed basis functions, which is why we introduced ABFs.

# How this works

KANs follow the Kolmogorov-Arnold Representation theorem, which simply states that any multivariate function, like a neural network can be decomposed to exactly become the summation of a function that is passed in, as an input, another sum over univariate functions.

Our implementation replaces basis function, that are static with adaptive that are fine-tuned during training, representing the univariate functions connecting each layer to layer.

Full research paper [here](https://drive.google.com/file/d/1qn3eyyuICa2K2_DajJhyqdH0dTrU3tM1/view?usp=sharing)

# Thanks
I would like to share my sincere thanks and appreciations to the following authors from where I get code snippets for my research:
 * Professor Matthew Johnson, Department of Engineering at University of Cambridge, for showing Fourier Feature Networks. Full repository can be found [here](https://github.com/matajoh/fourier_feature_nets)
 * Blealtan, for showing KAN network implementation. Full repository can be found [here](https://github.com/Blealtan/efficient-kan/tree/master)



# How to run

The ```pip install``` commands are already on the notebook, however, for running locally:

```pip install -r requirements.txt```

This notebook can be run in colab

And press run on the notebook
Any Questions: william1binki@gmail.com
