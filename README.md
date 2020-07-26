# Post-training Static Quantization (Pytorch)

This project perform post-training static quantization in Pytorch using ResNet18 architecture.

Configuration of Project Environment
=====================================

1. Clone the project.
2. Install packages required.
4. Run the notebook.

Setup procedure
----------------
1. Clone project from [GitHub](https://github.com/Sanjana7395/static_quantization.git).  
      Change to the directory static_quantization.
2. Install packages  
   In order to reproduce the code install the packages 

           pip install torch==1.5.1 
           pip install torchvision==0.6.1 
           pip install matplotlib

3. Run the notebook.  
      See **Documentation for the code** section for further details.
      In this notebook we use MNIST data set for experimenting.
      
Results
========

Below are the results obtained on the test set for the models trained in the project.

> NOTE    
   The results obtained are system specific. Due to different combinations of the neural 
   network cudnn library versions and NVIDIA driver library versions, the results can be 
   slightly different. To the best of my knowledge, upon reproducing the environment, the
   ballpark number will be close to the results obtained.

| Models                           | Accuracy (%)  | Memory size (MB)  | Inference time (ms)  |
|----------------------------------|:-------------:|:-----------------:|:--------------------:|
| Original                         | 99            | 44.76             | 13.46                |
| Quantized                        | 99            | 11.20             | 3.69                 |
