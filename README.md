# PIBLUP
PIBLUP is an application program for solving mixed model equations (MME), especially for very large ones. The core algorithm is preconditioned conjugate gradient (PCG) with preconditioner of block diagonal of MME, by iteration on data (IOD). To take full advantage of modern multicore and multiprocessor systems, two parallel computing strategies are applied in PIBLUP. Firstly, Intel Math Kernel Library (MKL) is employed (https://software.intel.com/en-us/intel-mkl) to accelerate mathematical operations. Secondly, we used shared memory programming introduced in Message Passing Interface Standard (MPI) Version 3.0. In a practical application, users can control both the Intel MKL threading and the number of MPI processes to optimally utilize computational resources. PIBLUP is written in C. The program will be actively maintained and new functions will be incorporated. If you have any questions and suggestions, please do not hesitate to contact us.

Directory program/ contains programs for PIBLUP v1.0. Examples (parameter file) in directory example/ are for PIBLUP 1.0.

Directory PIBLUPv1.1/ contains programs for PIBLUP v1.1 and its user manual. We added nearpd option to compute the nearest positive definite matrix of G in genoimc selection in PIBLUP v1.1. This leaded to a small change in syntax in parameter file.

Cite:
Kang, H, Ning, C, Zhou, L, Zhang, S, Yang, N, and J-F Liu (2018). PIBLUP: High-Performance Software for Large-Scale Genetic Evaluation of Animals and Plants. Frontiers in Genetics 9 (226).
