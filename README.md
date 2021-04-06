## KFusion-Opencl
This repo represents an optimized version of OpenCL KFusion implementation as appeared in SLAMBench open-source project.

The default OpenCL implementation of SLAMBench running at an NVidia GeForce GTX 770 and 'lr kt2' loop tajectory ran at 203 frames per second. 

This optimized version runs at 634 frames per second. 

### Info
You will need SLAMBench to make and run the code. Head to SLAMBench repo for more information on how to install it. 

https://github.com/pamela-project/slambench1

Use "run_slam" script to run this version of opencl implementation at slambench.

### Files
kfusion/src/opencl/* -> Optimized kernels and host

kfusion/include/constant_parameters.h -> Changed a constant

kfusion/src/benchmark.cpp -> Changed to fit optimizations


