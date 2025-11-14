# Advanced Topics on HPC, Supplementary Materials

This repo contains supplementary materials for the talk "Advanced Topics on High Performance Computing (HPC)".

1. Slides [[here](https://drive.google.com/file/d/1Y1Z59Io6bn8NxiwnGYqwLMt0tYDl9qol/view?usp=sharing)]
2. Hands-on: Nsight Guided Profiling [[here](https://github.com/j3soon/hpc-samples/blob/main/nsight-guided-profiling.md)]
   - Install [Nsight Systems](https://developer.nvidia.com/nsight-systems/get-started)
   - Install [Nsight Compute](https://developer.nvidia.com/tools-overview/nsight-compute/get-started)
   - Download sample [profile reports](https://github.com/j3soon/hpc-samples/releases)
3. Post-talk Survey [[here](https://forms.gle/mdfSg4CbNTFjQb1e9)]

## Abstract of the Talk

This session offers a practical overview of modern GPU trends and the core CUDA skills needed for high-performance development. We begin with a concise recap of current and emerging GPU directions, scaling laws, Huang's Law, NVLink/NVSwitch, GB200-class systems, and the growing support of low-precision emulation and MoE workloads. We then clarify how CUDA binaries and tools work in practice, covering PTX vs. SASS, portability, debugging and sanitizing tools, IDE integration, and workflow support through containers. The Nsight suite is introduced as the primary path to understanding real application behavior. Key CUDA optimization fundamentals are reviewed, including SIMT execution, memory hierarchy, memory coalescing, bank conflicts, vectorized access, synchronization, warp-level primitives, streams, and efficient atomics. The session concludes with a hands-on walkthrough of Nsight profiling results, applying guided profiling to explore ten concrete optimization opportunities. Participants should have the slides, Nsight Systems/Compute installed, and sample profile reports downloaded.

If time permits, we will extend the discussion into advanced CUDA optimization topics, including thread-block clusters (CGA), distributed shared memory, asynchronous barriers, asynchronous data movement, LDGSTS operations, tensor memory acceleration, and CUDA Graphs. We will also provide a brief tour of the NVIDIA HPC SDK, covering ISO C++, OpenMP/OpenACC, CUDA C++, CUDA Python, RAPIDS, cuPyNumeric, NVIDIA Warp, and the associated math (cuBLAS, CUTLASS, etc.) and core compute libraries (CCCL). Finally, we will review key NVIDIA communication libraries from HPC-X SDK, including CUDA-aware MPI with UCX, NCCL over NVLink, NVSHMEM and PGAS models, SHARP collectives, emerging NVLink-C2C memory coherence design, and GPUDirect Storage/RDMA.

## References

See [j3soon/hpc-notes](https://github.com/j3soon/hpc-notes/blob/master/nvidia-resources.md) for more references.
