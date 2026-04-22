# Advanced Topics on HPC, Supplementary Materials

This repo contains supplementary materials for the talk "Inside Modern GPUs: Emerging Trends, CUDA Optimization, and Profiling in Practice".

1. Slides [[here](https://drive.google.com/file/d/1YDa8GP21mBCRQk7o8_SI_Va7z5UW6Jbr/view?usp=drive_link)]
   - Old version (2025/12/08) [[here](https://drive.google.com/file/d/1mvr1AhyRmU6OVSrWiuR7nKbfSuEa2nM6/view?usp=sharing)]
   - Old version (2025/11/14) [[here](https://drive.google.com/file/d/1Y1Z59Io6bn8NxiwnGYqwLMt0tYDl9qol/view?usp=sharing)]
2. Hands-on: Nsight Guided Profiling [[here](https://github.com/j3soon/hpc-samples/blob/main/nsight-guided-profiling.md)]
   - Install [Nsight Systems](https://developer.nvidia.com/nsight-systems/get-started)
   - Install [Nsight Compute](https://developer.nvidia.com/tools-overview/nsight-compute/get-started)
   - Download sample [profile reports](https://github.com/j3soon/hpc-samples/releases)
3. Post-talk Survey [[here](https://forms.gle/UvJgqGmUDMVBxGSr5)]
4. Opencode with Free Nemotron 3 Super Setup [[here](https://github.com/j3soon/opencode-nemotron-free)]

## Abstract of the Talk

This session provides a practical introduction to modern GPU systems and the CUDA skills required for high-performance development. We begin with an overview of emerging industry trends, including scaling behaviors, advanced interconnects such as NVLink and NVSwitch, next-generation systems, and the growing role of low-precision computation, mixture-of-experts workloads, and low-latency inference.

Building on this context, we examine how CUDA works in practice, from compilation (PTX vs. SASS) to debugging, portability, and containerized development workflows. The Nsight toolchain is introduced as the primary means of understanding and optimizing application behavior on modern GPUs.

We then review key optimization fundamentals across execution, memory, and synchronization, including SIMT execution, efficient memory access patterns, and coordination across threads and warps. The session concludes with a hands-on walkthrough of Nsight profiling using a minimal example workload, where participants apply guided profiling to identify concrete optimization opportunities. Participants are encouraged to bring their own laptop with Nsight Systems and Nsight Compute pre-installed.

## (Extended) Abstract

This session offers a practical overview of modern GPU trends and the core CUDA skills needed for high-performance development. We begin with a concise recap of current and emerging GPU directions, scaling laws, Jensen's Law, NVLink/NVSwitch, GB200-class systems, and the growing support of low-precision emulation, MoE workloads, and low-latency inference with LPUs. We then clarify how CUDA binaries and tools work in practice, covering PTX vs. SASS, portability, debugging and sanitizing tools, IDE integration, and workflow support through containers. The Nsight suite is introduced as the primary path to understanding real application behavior. Key CUDA optimization fundamentals are reviewed, including SIMT execution, memory hierarchy, memory coalescing, bank conflicts, vectorized access, synchronization, warp-level primitives, streams, and efficient atomics. The session concludes with a hands-on walkthrough of Nsight profiling results, applying guided profiling to explore ten concrete optimization opportunities. Participants should bring their own laptop with Nsight Systems and Nsight Compute pre-installed.

If time permits, we will extend the discussion into advanced CUDA optimization topics, including thread-block clusters (CGA), distributed shared memory, asynchronous barriers, asynchronous data movement, LDGSTS operations, tensor memory acceleration, and CUDA Graphs. We will also provide a brief tour of the NVIDIA HPC SDK, covering ISO C++, OpenMP/OpenACC, CUDA C++, CUDA Python, RAPIDS, cuPyNumeric, NVIDIA Warp, and the associated math (cuBLAS, CUTLASS, etc.) and core compute libraries (CCCL). Finally, we will review key NVIDIA communication libraries from HPC-X SDK, including CUDA-aware MPI with UCX, NCCL over NVLink, NVSHMEM and PGAS models, SHARP collectives, emerging NVLink-C2C memory coherence design, and GPUDirect Storage/RDMA.

## References

See [j3soon/hpc-notes](https://github.com/j3soon/hpc-notes/blob/master/nvidia-resources.md) for more references.
