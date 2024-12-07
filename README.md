# Advanced Topics on HPC, Supplementary Materials

This repo contains supplementary materials for the talk "Advanced Topics on High Performance Computing (HPC)".

1. Post-talk Survey [[here](https://forms.gle/MiJ46yjHjr9rQUGi6)]
2. (Optional) Register GTC 2025 online for free [[here](https://www.nvidia.com/en-us/gtc/?ncid=GTC-NVMD8BQ6)]

## Introduction

The main goal of this talk is to introduce you to some of the latest NVIDIA technologies that I believe are most valuable for those learning CUDA & HPC. Given the limited time, we'll focus on providing a broad overview, so it's perfectly fine if you only take away a few key concepts.

## Useful Resources

For the topics you wish to explore further, start by consulting the official documentation, such as the [CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html) if you're aiming to become a "CUDA Ninja". However, official documentation can sometimes be challenging to understand. In such cases, searching for "NVIDIA Blog" and "GTC Talks" on relevant topics through Google often leads to excellent presentations and discussions on the subject. Also make sure to prioritize blogs and talks from recent years, as they are more likely to cover the latest technologies.

The following are the reference materials for further study.

## NVIDIA's Latest Hardware

- GB200 NVL72
  - [[Blog] NVIDIA Contributes NVIDIA GB200 NVL72 Designs to Open Compute Project](https://developer.nvidia.com/blog/nvidia-contributes-nvidia-gb200-nvl72-designs-to-open-compute-project/)
  - [[Blog] NVIDIA Ethernet Networking Accelerates World’s Largest AI Supercomputer, Built by xAI](https://nvidianews.nvidia.com/news/spectrum-x-ethernet-networking-xai-colossus)
- Grace Hopper & NVLink-C2C & Memory Coherent Architecture
  - [[Blog] NVIDIA Grace Hopper Superchip Architecture In-Depth](https://developer.nvidia.com/blog/nvidia-grace-hopper-superchip-architecture-in-depth/)
  - [[Blog] NVIDIA GH200 Superchip Accelerates Inference by 2x in Multiturn Interactions with Llama Models](https://developer.nvidia.com/blog/nvidia-gh200-superchip-accelerates-inference-by-2x-in-multiturn-interactions-with-llama-models/)
  - [[GitHub] Memory Coherent Architecture](https://github.com/j3soon/nways_accelerated_programming/blob/main/_basic/memory_coherent/jupyter_notebook/memory_coherent_architectures.ipynb)
- GPUDirect Storage & RDMA
  - [NVIDIA GPUDirect](https://developer.nvidia.com/gpudirect)
- DGX SuperPOD
  - [NVIDIA DGX SuperPOD: Next Generation Scalable Infrastructure for AI Leadership Reference Architecture Featuring NVIDIA DGX H100](https://docs.nvidia.com/dgx-superpod/reference-architecture-scalable-infrastructure-h100/latest/index.html)
  - [NVIDIA DGX SuperPOD FAQ](https://docs.nvidia.com/dgx-superpod/faq/latest/dgx-superpod.html)

## CUDA & Optimization

- [CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html)
- [[GitHub] NVIDIA/cuda-samples](https://github.com/NVIDIA/cuda-samples)
- Coalesced Memory Access
  - [[Blog] How to Access Global Memory Efficiently in CUDA C/C++ Kernels](https://developer.nvidia.com/blog/how-access-global-memory-efficiently-cuda-c-kernels/)
  - [5.3.2. Device Memory Accesses \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#device-memory-accesses)
- Shared Memory Bank Conflict
  - [[Blog] Using Shared Memory in CUDA C/C++](https://developer.nvidia.com/blog/using-shared-memory-cuda-cc/)
  - [[Blog] An Efficient Matrix Transpose in CUDA C/C++](https://developer.nvidia.com/blog/efficient-matrix-transpose-cuda-cc/)
  - [16.4.3. Shared Memory \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#shared-memory-5-x)
- CUDA Streams
  - [[Blog] How to Optimize Data Transfers in CUDA C/C++](https://developer.nvidia.com/blog/how-optimize-data-transfers-cuda-cc/)
  - [[Blog] How to Overlap Data Transfers in CUDA C/C++](https://developer.nvidia.com/blog/how-overlap-data-transfers-cuda-cc/)
  - [[Blog] GPU Pro Tip: CUDA 7 Streams Simplify Concurrency](https://developer.nvidia.com/blog/gpu-pro-tip-cuda-7-streams-simplify-concurrency/)
  - [[Blog] Using the NVIDIA CUDA Stream-Ordered Memory Allocator, Part 1](https://developer.nvidia.com/blog/using-cuda-stream-ordered-memory-allocator-part-1/)
  - [[Blog] Using the NVIDIA CUDA Stream-Ordered Memory Allocator, Part 2](https://developer.nvidia.com/blog/using-cuda-stream-ordered-memory-allocator-part-2/)
  - [9.2.1.4. Streams and Events \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#streams-and-events)
  - [11. Stream Ordered Memory Allocator \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#stream-ordered-memory-allocator)
- Atomics
  - [[Blog] CUDA Pro Tip: Optimized Filtering with Warp-Aggregated Atomics](https://developer.nvidia.com/blog/cuda-pro-tip-optimized-filtering-warp-aggregated-atomics/)
  - [7.14. Atomic Functions \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions)
- Vectorized Memory Access
  - [[Blog] CUDA Pro Tip: Increase Performance with Vectorized Memory Access](https://developer.nvidia.com/blog/cuda-pro-tip-increase-performance-with-vectorized-memory-access/)
- Warp-Level Primitives
  - [[Blog] Using CUDA Warp-Level Primitives](https://developer.nvidia.com/blog/using-cuda-warp-level-primitives/)
  - [7.19. Warp Vote Functions \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#warp-vote-functions)
  - [7.20. Warp Match Functions \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#warp-match-functions)
  - [7.21. Warp Reduce Functions \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#warp-reduce-functions)
  - [7.22. Warp Shuffle Functions \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#warp-shuffle-functions)

## Advanced CUDA

- PTX (Parallel Thread Execution) and SASS (Streaming Assembly)
  - [PTX and SASS Assembly Debugging](https://docs.nvidia.com/nsight-visual-studio-edition/cuda-advanced-topics/index.html#ptx-and-sass-assembly-debugging)
  - [CUDA Binary Utilities](https://docs.nvidia.com/cuda/cuda-binary-utilities/index.html)
- Cooperative Groups (CG)
  - [[Blog] Cooperative Groups: Flexible CUDA Thread Programming](https://developer.nvidia.com/blog/cooperative-groups/)
  - [8. Cooperative Groups \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#cooperative-groups)
- LDGSTS
  > Require Ampere architecture or later.
  - [[Blog] NVIDIA Ampere Architecture In-Depth](https://developer.nvidia.com/blog/nvidia-ampere-architecture-in-depth/)
  - [[Blog] Controlling Data Movement to Boost Performance on the NVIDIA Ampere Architecture](https://developer.nvidia.com/blog/controlling-data-movement-to-boost-performance-on-ampere-architecture/)
  - [[Blog] Boosting Application Performance with GPU Memory Prefetching](https://developer.nvidia.com/blog/boosting-application-performance-with-gpu-memory-prefetching/)
  - [7.26. Asynchronous Barrier \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#aw-barrier)
  - [7.27. Asynchronous Data Copies \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#asynchronous-data-copies)
  - [7.28. Asynchronous Data Copies using `cuda::pipeline`](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#asynchronous-data-copies-using-cuda-pipeline)
- Hopper Architecture & Thread Block Cluster & Distributed Shared Memory (DSMEM) & Tensor Memory Accelerator (TMA)
  > Require Hopper architecture or later.
  - [[Blog] NVIDIA Hopper Architecture In-Depth](https://developer.nvidia.com/blog/nvidia-hopper-architecture-in-depth/)
  - [2.3. Memory Hierarchy \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#memory-hierarchy)
  - [3.2.5. Distributed Shared Memory \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#distributed-shared-memory)
  - [7.29. Asynchronous Data Copies using the Tensor Memory Accelerator (TMA) \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#asynchronous-data-copies-using-the-tensor-memory-accelerator-tma)
- CUDA Graphs
  - [[Blog] Getting Started with CUDA Graphs](https://developer.nvidia.com/blog/cuda-graphs/)
  - [[Blog] Employing CUDA Graphs in a Dynamic Environment](https://developer.nvidia.com/blog/employing-cuda-graphs-in-a-dynamic-environment/)
  - [[Blog] Constructing CUDA Graphs with Dynamic Parameters](https://developer.nvidia.com/blog/constructing-cuda-graphs-with-dynamic-parameters/)
  - [[Blog] Enabling Dynamic Control Flow in CUDA Graphs with Device Graph Launch](https://developer.nvidia.com/blog/enabling-dynamic-control-flow-in-cuda-graphs-with-device-graph-launch/)
  - [[Blog] Dynamic Control Flow in CUDA Graphs with Conditional Nodes](https://developer.nvidia.com/blog/dynamic-control-flow-in-cuda-graphs-with-conditional-nodes/)
  - [[Blog] Optimizing llama.cpp AI Inference with CUDA Graphs](https://developer.nvidia.com/blog/optimizing-llama-cpp-ai-inference-with-cuda-graphs/)
  - [3.2.8.7. CUDA Graphs \| CUDA C++ Programming Guide](https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#cuda-graphs)

## NVIDIA HPC SDK

- ISO C++/Fortran, OpenACC/OpenMP, CUDA
  - [[GitHub] N-ways to GPU programming](https://github.com/j3soon/nways_accelerated_programming)
- Python
  - [[Blog] RAPIDS cuDF Accelerates pandas Nearly 150x with Zero Code Changes](https://developer.nvidia.com/blog/rapids-cudf-accelerates-pandas-nearly-150x-with-zero-code-changes/)
  - [[Blog] Faster HDBSCAN Soft Clustering with RAPIDS cuML](https://developer.nvidia.com/blog/faster-hdbscan-soft-clustering-with-rapids-cuml/)
  - [[Blog] Unifying the CUDA Python Ecosystem](https://developer.nvidia.com/blog/unifying-the-cuda-python-ecosystem/)
  - [[Blog] Effortlessly Scale NumPy from Laptops to Supercomputers with NVIDIA cuPyNumeric](https://developer.nvidia.com/blog/effortlessly-scale-numpy-from-laptops-to-supercomputers-with-nvidia-cupynumeric/)
  - [[Blog] Creating Differentiable Graphics and Physics Simulation in Python with NVIDIA Warp](https://developer.nvidia.com/blog/creating-differentiable-graphics-and-physics-simulation-in-python-with-nvidia-warp/)
- [NVIDIA CUDA-X Libraries](https://developer.nvidia.com/gpu-accelerated-libraries)
  - [[Blog] Accelerating GPU Applications with NVIDIA Math Libraries](https://developer.nvidia.com/blog/accelerating-gpu-applications-with-nvidia-math-libraries/)
- [CUDA C++ Core Libraries](https://nvidia.github.io/cccl/cpp.html) and [`stdexec`](https://nvidia.github.io/stdexec/)
- NVSHMEM
  - [[Blog] Scaling Scientific Computing with NVSHMEM](https://developer.nvidia.com/blog/scaling-scientific-computing-with-nvshmem/)
- NVIDIA Collective Communications Library (NCCL)
  - [[Blog] Fast Multi-GPU collectives with NCCL](https://developer.nvidia.com/blog/fast-multi-gpu-collectives-nccl/)
  - [[Blog] Doubling all2all Performance with NVIDIA Collective Communication Library 2.12](https://developer.nvidia.com/blog/doubling-all2all-performance-with-nvidia-collective-communication-library-2-12/)
- NVIDIA Scalable Hierarchical Aggregation and Reduction Protocol (SHARP)
  - [[Blog] Advancing Performance with NVIDIA SHARP In-Network Computing](https://developer.nvidia.com/blog/advancing-performance-with-nvidia-sharp-in-network-computing/)
  - [[YouTube] In-Network Computing with NVIDIA SHARP](https://youtu.be/uzYZP_z_5WE)

## Dev Tools

- Compute Sanitizer
  - [[Blog] Efficient CUDA Debugging: Memory Initialization and Thread Synchronization with NVIDIA Compute Sanitizer](https://developer.nvidia.com/blog/efficient-cuda-debugging-memory-initialization-and-thread-synchronization-with-nvidia-compute-sanitizer/)
  - [Compute Sanitizer](https://docs.nvidia.com/compute-sanitizer/ComputeSanitizer)
- Nsight Systems/Compute/Graphics & [Nsight Visual Studio Code Edition](https://developer.nvidia.com/nsight-visual-studio-code-edition)
  - [[GitHub] NVIDIA/nsight-vscode-edition](https://github.com/NVIDIA/nsight-vscode-edition)
  - [and more](https://developer.nvidia.com/tools-overview).
- Containerization
  - [[GitHub] NVIDIA Docker](NVIDIA/nvidia-container-toolkit)
  - [[GitHub] Singularity](https://github.com/sylabs/singularity) & [[GitHub] Apptainer](https://github.com/apptainer/apptainer)
  - [[GitHub] ENROOT](https://github.com/NVIDIA/enroot) & [[GitHub] Pyxis](https://github.com/NVIDIA/pyxis)

## Higher-Level SDKs

- NVIDIA NeMo
  - [[GitHub] NVIDIA/NeMo](https://github.com/NVIDIA/NeMo)

- NVIDIA Omniverse & Isaac
  - [[GitHub] NVIDIA Isaac Summary](https://github.com/j3soon/nvidia-isaac-summary)

## Other GTC Talks

- [GTC 24 - Advanced Performance Optimization in CUDA - S62192](https://www.nvidia.com/en-us/on-demand/session/gtc24-s62192/)
- [GTC 24 - CUDA, New Features and Beyond - S62400](https://www.nvidia.com/en-us/on-demand/session/gtc24-s62400/)
- [GTC 24 - How To Write A CUDA Program, The Ninja Edition - S62401](https://www.nvidia.com/en-us/on-demand/session/gtc24-s62401/)
- [GTC 24 - Introduction to CUDA Programming and Performance Optimization - S62191](https://www.nvidia.com/en-us/on-demand/session/gtc24-s62191/)
- [GTC 24 - Multi GPU Programming Models for HPC and AI - S61339](https://www.nvidia.com/en-us/on-demand/session/gtc24-s61339/)
- [GTC 24 - Warp, Advancing Simulation AI with Differentiable GPU Computing in Python - S63345](https://www.nvidia.com/en-us/on-demand/session/gtc24-s63345/)
- [GTC Spring 23 - Connect with the Experts, C++ Standard Parallelism and C++ Core Compute Libraries - CWES52064](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-cwes52064)
- [GTC Spring 23 - C++ Standard Parallelism - S51755](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-s51755/)
- [GTC Spring 23 - CUDA, New Features and Beyond - S51225](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-s51225/)
- [GTC Spring 23 - Robust and Efficient CUDA C++ Concurrency with Stream-Ordered Allocation - S51897](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-s51897/)
- [GTC Spring 22 - C++ Standard Parallelism - S41960](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s41960/)
- [GTC Spring 22 - How CUDA Programming Works - S41487](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s41487/)
- [GTC Spring 22 - How to Understand and Optimize Shared Memory Accesses using Nsight Compute - S41723](https://www.nvidia.com/en-us/on-demand/session/gtcspring22-s41723/)
- [GTC Fall 21 - Accelerate Computing with CUDA Python - A31138](https://www.nvidia.com/en-us/on-demand/session/gtcfall21-a31138/)
- [GTC Fall 21 - GPU Acceleration in Python using CuPy and Numba - A31149](https://www.nvidia.com/en-us/on-demand/session/gtcfall21-a31149/)
- [GTC Fall 21 - Legate, Scaling the Python Ecosystem - A31168](https://www.nvidia.com/en-us/on-demand/session/gtcfall21-a31168/)
- [GTC Spring 21 - How GPU Computing Works - S31151](https://www.nvidia.com/en-us/on-demand/session/gtcspring21-s31151/)
