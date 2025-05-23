# Learning Smooth Dendrite Morphological Neurons by Stochastic Gradient Descent for Pattern Classification

Learning algorithms for dendrite morphological neurons (DMNs) generally do not employ standard machine learning (ML) methods, such as stochastic gradient descent (SGD), because the morphological operations, maximum and minimum, are non-differentiable. Notice that using SGD requires calculating the partial derivatives of the loss function with respect to the learnable parameters to obtain the delta rules.

To overcome this issue, we propose using smooth morphological operations based on the exponential function, which is differentiable, to learn DMNs via SGD. We use a DMN topology that comprises spherical dendrites, smooth maximum activation function nodes, and a softmax output layer. The location of a spherical dendrite in the input space is given by its centroid. Hence, we derive the delta rules for adjusting the dendrites' centroids and the output layer weights by minimizing the cross-entropy loss function under an SGD scheme.

Here, we provide the MATLAB codes of our proposed approach. Two demos were prepared. The first one (demo_dsn.m) runs the DMN's learning and shows the results on 2D synthetic datasets, such as the image below. The second demo (demo_bayesopt.) shows how to automatically tune the DMN hyperparameters (smoothness factor and learning rate) using Bayesian optimization, a method widely used in artificial neural networks.

Please cite the following articles:
1. Wilfrido Gómez-Flores and Humberto Sossa. Learning Smooth Dendrite Morphological Neurons by Stochastic Gradient Descent for Pattern Classification, Neural Networks, vol. 168, pp. 665-676, 2023. (https://doi.org/10.1016/j.neunet.2023.09.033)
2. Wilfrido Gómez-Flores and Humberto Sossa. Smooth Dendrite Morphological Neurons, Neural Networks, vol. 136, pp. 40-53, 2021. (https://doi.org/10.1016/j.neunet.2020.12.021)


![picture alt](https://github.com/wgomezf/DMN_SGD/blob/main/dsn.png "DSN")
