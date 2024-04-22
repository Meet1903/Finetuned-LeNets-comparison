# FineTuned LeNet-5 models & comparison

---

## Overview

LeNet is a convolutional neural network structure proposed by LeCun et al. in 1998. In general, LeNet refers to LeNet-5 and is a simple convolutional neural network


## Dataset Overview
[MNIST](https://github.com/datapythonista/mnist) - Yann LeCun

The MNIST database is a dataset of handwritten digits. It has 60,000 training samples, and 10,000 test samples. Each image is represented by 28x28 pixels, each containing a value 0 - 255 with its grayscale value.

Example:

![Image](/images/MNIST.png)

## Run the program
Execute the LeNets.ipynb file directly. Each distinct model is separated, allowing for individual execution as well

## Result:

### Version 1:  Batch Normalization in the hidden layers, Standard Normalization for the input layer.

Loss & Accuracy

![Image](/images/v1_acc.png)

batch norm parameters for each layer

![Image](/images/v1_batchNorm.png)

### Version 2:  Batch Normalization for the input layer too.

Loss & Accuracy

![Image](/images/v2_acc.png)

batch norm parameters for each layer

![Image](/images/v2_batchNorm.png)

### Version 3:  DropOut instead of Batch Normalization

Loss & Accuracy

![Image](/images/v3_acc.png)

### Version 4:  Both Drop Out and Batch Normalization

Loss & Accuracy

![Image](/images/v4_acc.png)

batch norm parameters for each layer

![Image](/images/v4_batchNorm.png)

### Final result comparison:
| Model Version | Accuracy | Loss |
|----------|----------|----------|
| Version 1   | 98.7    | 1.4851    |
| Version 2    | 98.64   | 1.4853   |
| Version 3    | 68.05   | 1.8180    |
| Version 4    | 82.09    | 1.6769   |
