---
title: OBPMark
description: On-Board Processing Benchmarks
---

![ESA logo](/assets/esa-logo.png)
![BSC logo](/assets/bsc-logo.png)


What is OBPMark?
---------------------
OBPMark (On-Board Processing Benchmarks) is a set of computational performance benchmarks developed specifically for spacecraft on-board data processing applications, such as: image and radar processing, data and image compressions, signal processing and machine learning.

The development of OBPMark was driven by the lack of openly available and representative benchmarks for space applications.

### Benchmarks
OBPMark is split into three sets of on-board processing benchmarks, each with its own repository:

FIXME make this into a table

[OBPMark](https://github.com/OBPMark/OBPMark) -- Application level benchmarks, "classical" processing.
OBPMark-ML (TODO add link) -- Application level benchmark for machine learning based processing. 
[OBPMark-Kernels (GPU4S Bench)](https://github.com/OBPMark/GPU4S_Bench) -- Processing building blocks

### Objectives


### Description

OBPMark consists of the following main components: 
1. A technical note describing the benchmarks, their implementation and result reporting. 
2. Reference implementations in C (sequential) and standard parallelisation schemes, such as OpenMP, OpenCL and CUDA. 
3. A list of known published performance benchmark results. 

OBPMark has been developed in cooperation by the European Space Agency (ESA) and Barcelona Supercomputing Center (BSC). 
The OBPMark definition and implementation has been made available partially through funding from the ESA "General Studies Programme (GSP)".

OBPMark is openly available, and contributions from the community are warmly welcome. 

### Contact

Contact: OBPMark@esa.int  
  
Authors/Chairs:  
David Steenari, European Space Agency (ESA)  
Dr. Leonidas Kosmidis, Barcelona Supercomputing Center (BSC)  

### Contributors

Contributors:  
Alvaro Jover-Alvarez, Universitat Politècnica de Catalunya (UPC) / Barcelona Supercomputing Center (BSC)

Ivan Rodriguez-Ferrandez, Universitat Politècnica de Catalunya (UPC) / Barcelona Supercomputing Center (BSC).

