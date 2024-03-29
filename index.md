---
title: OBPMark
descrption: On-Board Processing Benchmarks
---

What is OBPMark?
---------------------
OBPMark (On-Board Processing Benchmarks) is a set of computational performance benchmarks developed specifically for spacecraft on-board data processing applications, such as: image and radar processing, data and image compressions, signal processing and machine learning.

The development of OBPMark was driven by the lack of openly available and representative benchmarks for space applications.

OBPMark consists of three main components: 
1. A technical note describing the benchmarks, their implementation and result reporting. 
2. Reference implementations in C (sequential) and standard parallelisation schemes, such as OpenMP, OpenCL and CUDA. 
3. A list of known published performance benchmark results. 

OBPMark has been developed in cooperation by the European Space Agency (ESA) and Barcelona Supercomputing Center (BSC). 
The OBPMark definition and implementation has been made available partially through funding from the ESA "General Studies Programme (GSP)".

OBPMark is openly available, and contributions from the community are warmly welcome. 

### Repositories

[OBPMark Repository](https://github.com/OBPMark/OBPMark) 

[GPU4S Bench - OBPMark-Kernel Repository](https://github.com/OBPMark/GPU4S_Bench)

### Contact

Contact: OBPMark@esa.int  
  
Authors/Chairs:  
- David Steenari, European Space Agency (ESA)  
- Dr. Leonidas Kosmidis, Barcelona Supercomputing Center (BSC)  

### Contributors

Contributors:   
- Ivan Rodriguez Ferrandez, Universitat Politècnica de Catalunya and Barcelona Supercomputing Center (UPC/BSC):
	- Implementation of Benchmark #1.1 "Image Calibration and Correction"
	- Implementation of Benchmark #2.1 "CCSDS 121.0 Data Compression"
	- Implementation of Benchmark #2.2 "CCSDS 122.0 Image Compression"
	- Verification of implementations.
- Alvaro Jover-Alvarez, Universitat Politècnica de Catalunya and Barcelona Supercomputing Center (UPC/BSC):
	- Implementation of OpenMP versions of Benchmarks #1.1, #2.1, .
- Marc Solé Bonet, Barcelona Supercomputing Centrer (BSC):
	- Implementation of Benchmark #3.1 "AES Encryption"
	- Implementation of Benchmark #1.2 "Radar Image Processing"
  
## Release Notice
Please note that OBPMark is currently in "Public Beta" while the implementations and verifications of the benchmarks are being completed.

Expect features and data to be missing. For an overview of the main current issues and missing features, see the "Issues" tab in the git repository.

In the meanwhile, users are invited to test out the existing implementations (see list below) and report bugs and issues via the github interface.

## Description
This repository contains a set of reference implementations for performing benchmarks on devices and systems on-board spacecraft. 

The following folders are in the repository: 

	docs/	The TeX files for building the OBPMark specification. 
	src/	Source files for each of the benchmarks. 

The benchmarks are organised in the following structure ("Private Beta" current status also shown): 

	src/1.1-image/				-- Available in C (sequential), OpenMP, OpenCL and CUDA.
	src/1.2-radar/				-- Available in C (sequential), OpenMP, OpenCL and CUDA.
	src/2.1-data_compression/		-- Available in C (sequential), OpenMP, OpenCL and CUDA.
	src/2.2-image_compression/		-- Available in C (sequential), OpenMP, OpenCL and CUDA.
	src/2.3-hyperspectral_compression/	-- Not available yet.
	src/3.1-aes_encryption/			-- Not available yet.
	src/common/

The entire set of benchmarks can be built by invoking the Makefile in the top src/ directory, or by invoking the individual Makefiles in each of the src sub-directories. 

For detailed build instructions see [Build Instructions](build_instructions.md) 

