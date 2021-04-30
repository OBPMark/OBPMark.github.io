# Build instructions

The entire set of benchmarks can be built by invoking the Makefile in the top src/ directory, or by invoking the individual Makefiles in each of the src sub-directories.

## Dependencies

The following packages are optional: 
- OpenMP
- OpenCL
- CUDA
- (HIP)

## Build Options 

Per default, the (sequential) C version is built.

Use of parallelisation schemes can be done by specifying the target framework for the make command: 

make openmp
make opencl 
make cuda 
(make hip) 


## Run Instructions

After successful build, binary executables can be found in the bin folder in each benchmark directory.
