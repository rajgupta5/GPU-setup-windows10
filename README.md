# GPU-setup-windows10

- https://www.youtube.com/watch?v=StH5YNrY0mE

## Steps to Instsll Cuda Toolkit and CuDNN for Deep Learning ##
- Download Cuda Toolkit 10.0 and install it
  - https://developer.nvidia.com/cuda-10.0-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exelocal
- Download Cudnn library for the same version in C:/
  - https://developer.nvidia.com/rdp/cudnn-archive
  - Download cuDNN v7.6.5 (November 5th, 2019), for CUDA 10.0
- Set the path in the environment variable for bin, lib, include folders
- Download visual studio 2017 , everything related to c++
- create an environment, then install tensorflow-gpu
  - conda create -n gputest python==3.6
  - conda activate gputest
  - pip install tensorflow-gpu==2.0.0
  - python
  - import tensoflow as tf (this will be seen: Successfully opened dynamic library cudart64_100.dll)
  - tf.test.is_gpu_available()
  - tf.test.is_built_with_cuda()
