# Split-Kernals

## Problem Statement:
1. Implement a CNN from scratch for Classification of objects for
CIFAR 100 Dataset
2. Implement a Split Kernel CNN for above built architecture
3. Compare the accuracy and Time taken.

## What are Split Kernels ? 
  1. A spatial separable convolution simply divides a kernel into two, smaller
  kernels.
  2. Example : 
   
  
  <img src="https://miro.medium.com/max/1400/1*mL53fW0tJpNWEePp54y1Sg.png" width="700" height="150">
  
  
  A spatial separable convolution simply divides a kernel into two, smaller kernels. The most common case would be to divide a 3x3 kernel into a 3x1 and 1x3 kernel, like so:

  
  <img src="https://miro.medium.com/max/1400/1*o3mKhG3nHS-1dWa_plCeFw.png" width="600" height="400">
   
  
  ## Advantages Of Split Kernels
1. Number of Calculations done are reduced.In the above example instead of doing one convolution with 9 multiplications, we
do two convolutions with 3 multiplications each (6 in total) to achieve the same
effect.
2. With less calculations, computational complexity goes down, and the network
is able to run faster
3. Splits kernels helps in decreasing no of parameters to calculate. But the issue
with split kernels is that all the kernels cannot be separated into two parts.
