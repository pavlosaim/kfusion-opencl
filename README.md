## KFusion-Opencl
This repo represents an optimized version of OpenCL KFusion (A Visual SLAM algorithm) implementation as appeared in SLAMBench open-source project.

The evaluation was done on an NVidia GeForce GTX 770 GPU, running the ICL-NUIM data set "lr kt2" loop.

The default KFusion of SLAMBench ran at 203 frames per second and 18.118m ATE.

This optimized version ran at 634 frames per second and 19.38m ATE. 

### Info
You will need SLAMBench to make and run the code. Head to SLAMBench repo for more information on how to install it. 

https://github.com/pamela-project/slambench1

We also used the living room trajectory as input in a raw format. It an be installed as follows:
<pre><code>mkdir living_room_traj2_loop
cd living_room_traj2_loop
wget http://www.doc.ic.ac.uk/~ahanda/living_room_traj2_loop.tgz
tar xzf living_room_traj2_loop.tgz
./build/kfusion/thirdparty/scene2raw living_room_traj2_loop living_room_traj2_loop.raw
</code></pre>

Use "run_slam" script to run this version of opencl implementation at slambench.

### Files
kfusion/src/opencl/* -> Optimized kernels and host

kfusion/include/constant_parameters.h -> Changed a constant

kfusion/src/benchmark.cpp -> Changed to fit optimizations


