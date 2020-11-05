cmake_minimum_required(VERSION 3.9 FATAL_ERROR)

set(CMAKE_CUDA_COMPILER "/usr/local/cuda-10.2/bin/nvcc") 
#set(CMAKE_CUDA_COMPILER "/usr/local/cuda/bin/nvcc") 
# PATH="$PATH:/home/workdir" 
# export PATH="$PATH:/usr/local/cuda/bin"


project(helloCuda LANGUAGES CUDA)
#project(helloCuda LANGUAGES C CXX CUDA) 


message("PROJECT_NAME: ${PROJECT_NAME}")
message("CMAKE_SOURCE_DIR: ${CMAKE_SOURCE_DIR}") 

#target_compile_features(hello-cuda PUBLIC cxx_std_11)
add_executable(helloCuda helloCuda.cu) 


