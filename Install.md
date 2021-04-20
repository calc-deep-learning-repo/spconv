
## 2. Common Problems

### 2.1 CMake Error: Could not find cmake module file: CMakeCUDAInformation.cmake

```bash
set(CMAKE_CUDA_COMPILER  /home/sukie/program/cuda-10.1/bin/nvcc)
find_package(CUDA)
include_directories(/home/sukie/program/cuda-10.1/include)
```

### 2.2 CMake Error: CMake can not determine linker language for target: spconv_nms

```cmake
set_target_properties(spconv_nms PROPERTIES LINKER_LANGUAGE CXX)
```

### 2.3 Could not find cuDNN

```cmake
set(CUDNN_INCLUDE_DIR /home/sukie/program/cuda/include)
set(CUDNN_LIBRARY /home/sukie/program/cuda/lib64)
```

```cmake
set(CMAKE_PREFIX_PATH /home/sukie/program/cuda)
set(CUDNN_DIR)
```

### 2.4 /usr/bin/ld: cannot find /home/sukie/program/cuda-10.1/lib64/: File format not recognized

