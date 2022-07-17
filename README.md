# Binarized Neural Networks
Binarized Neural Networks (BNN) are neural networks very efficient, since its implementation can be done operating completely using bitwise operations, highly optimized in current processors.

Their peculiarity is to have binary weights, which in particular can have values in {-1,1}.

However, this causes the network to be non-differentiable, and therefore they are not easily trainable.

With this project, the BNN is trained encoding the problem as a propositional MaxSAT logic problem, which then will be solved using the RC2 solver from PySAT.

In particular, the activation function of the BNN considered is the following:

![](https://latex.codecogs.com/png.latex?%5Cdpi%7B300%7D%20%5Chuge%20out%5E%7B%28i%29%7D%20%3D%20sign%28%5Csum_%7Bj%3D0%7D%5Em%20w_j%20x_j%5E%7B%28i%29%7D%29%20%5Cin%20%5C%7B-1%2C%201%5C%7D)

## Contents
In the repository can be found a PDF file with the presentation fo the project and its solution (definition, encoding, constraints, solution and analysis)

In the Jupyter notebook can be found the implementation of such problem using PySAT