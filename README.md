# mat1510_project

This is a review of the paper "An Empirical Study of Example Forgetting during Deep Neural Network Learning" 
by Mariya Toneva, Alessandro Sordoni, Remi Tachet des Combes, Adam Trischler, Yoshua Bengio, Geoffrey J. Gordon. ()

I tried two novel experiments based on the results of the paper:
1) train the same network on modified MNIST (cutting out a 8x8 pixel square in each of the quardrant in each image) 
and identify which part is most deterministic for each digit class
2) obtain the indices of forgettable examples using the algorithm presented in the paper, then train the same network on MNIST 
with forgettable examples removed to verify the importance of forgettable examples in classification accuracy

The code for identifying forgettable examples and calculating forgetting statistics are adapted from the original paper. 
(https://github.com/mtoneva/example_forgetting)

Reference:
Toneva, M., Sordoni, A., Combes, R. T. des, Trischler, A., Bengio, Y., &amp; Gordon, G. J. (2019). An
empirical study of example forgetting during deep neural network learning. arXiv.org. arXiv:1812.05159.
URL https://doi.org/10.48550/arXiv.1812.05159
