# CNN attempt in CUDA

A CUDA version of convolutional neural network LeNet-5

## Files

### network.h

1.Structures needed for CNN implementation

2.Host functions definced to be used to implement this project

### convolution.cu

A small copy of convolution implementation in CUDA

### network.cu

1.Kernel functions about detailed implementations of network

2.Host functions to set up network structure

3.Host functions which can be controlled outside to implement this network

### cnn.cu

Main function to implement this network

## Implementation

nvcc main.cu convolution.cu -Xcompiler -O3 -Xcompiler -Wall -Xptxas -O3 -o task

./task $batch $epoch $learning_rate
