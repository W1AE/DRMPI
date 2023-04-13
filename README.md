# DRMPI

## Abstract:

A popular approach for parameter optimization in multilayer Moore-Penrose inverse (MPI) methods is the least-square strategy, which has shown impressive performance in a wide range of tasks. However, the conventional method for constructing deep MPI structures involves building the architecture layer-by-layer, which can lead to inefficient use of information and poor data propagation. In order to solve this limitation, the authors drew inspiration from the shortcut connections to create a very deep network called the deep residual MPI network (DRMPN). In particular, the DRMPN is an iterative learning method. In other words, the method learns the optimal features from the input data with several epochs. In each iteration, the proposed method adds one feature reinforcement block (FRB) into the structure to learn the optimal representation and to map the data to the output space (get a label). The experimental results with varying training samples (from $3\,K$ to $1.8\,M$) show that the proposed models provide higher Top-1 testing accuracy than most representation learning algorithms.

## Contributions:
* I. Architecture side -  Two novel LS-based algorithms called RML-MP and SRML-MP are proposed. Specifically, i) to enhance the discriminitively of the latent space features, the RML-MP is developed; ii) the global-level representations of input pattern are generated through the proposed SRML-MP strategy.

* II. Application side - The key contribution of this paper in terms of its application is the usage of OC-SNN and MCOC-SNN, which harnesses high-level abstract features to handle large-scale datasets such as ImageNet and Place365. Furthermore, the cross-domain validations verify the effectiveness of the proposed methods. 

## Learning Structure:

<img src="https://github.com/W1AE/Retraining/blob/main/f.jpg" width="550" height="330" />
Fig. 1 Flowchart of the RML-MP and SRML-MP for multi-view representation learning.

<img src="https://github.com/W1AE/Retraining/blob/main/f1.jpg" width="1050" height="430" />
Fig.2 Comparison of frameworks of the (a) M-ELM, (b) RML-ELM, and (c) SRML-ELM. The difference of RML-ELM and SRML-ELM lies in Stage 3, the RML-ELM use $\ell_2$ penalty to recalculate the parameters while the SRML-ELM adopt $\ell_{1/2}$ penalty to update the weights.

## Related Work:

[1] Arvix: Multi-Model Least Square-Based Recomputation Framework for Large Data Analysis. 

## Downloads:
### Caltech-101 (Image Classification Domain)
* Caltech-101 dataset: [Caltech-101 DATASET](http://www.vision.caltech.edu/Image_Datasets/Caltech101/)
* Caltech-101 Inception-v3 features: [Caltech-101-testing (GoogLe Drive)](https://drive.google.com/file/d/1W_AFsaCgUdP1rBRnsjS24dWPW9MYCbAQ/view?usp=sharing) [Caltech-101-training (GoogLe Drive)](https://drive.google.com/file/d/1HWK9COAeQFOE4j6Z5wtfvJpkFneVm50Y/view?usp=sharing)
* Source code for Caltech-101: [Caltech-101](https://github.com/W1AE/Retraining/blob/main/Demo_Caltech101.zip)
### MNIST-2 (One Class Classification Domain)
* MNIST dataset: [MNIST DATASET](http://yann.lecun.com/exdb/mnist/)
* MNIST-2 features: [MNIST-2 (GoogLe Drive)](https://drive.google.com/file/d/1kWEMoIbtR8TKJq0X8btXrFqSetzOyHWH/view?usp=sharing) or [MNIST-2 (GitHub)](https://github.com/W1AE/Retraining/blob/main/M_2.mat)
* Source code for MNIST-2: [OC-MNIST-2](https://github.com/W1AE/Retraining/blob/main/Demo_MNIST.zip)

## Dependancies
* Matlab version 2020a,
* A workstation with a 256GB memory and an E5-2650 processor.

## Reproduce the Experimental Results

#The code is released in content-obscured version (p files). After acceptance of the manuscript (if decided so), the source code will be made public.

