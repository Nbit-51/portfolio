# Navaneeth Singh

**Computer Science Student · ML Systems · Inference Engineering · Systems Programming**

I’m a third-year Computer Science student at JSS Academy of Technical Education, Bengaluru, interested in how machine-learning models actually execute on real hardware.

My current work sits at the intersection of **deep learning and low-level systems**: GPU kernels, CPU inference runtimes, quantization, memory bandwidth, KV-cache behavior, SIMD, and efficient model deployment.

I learn best by building a system, measuring it, finding the bottleneck, and then studying why that bottleneck exists.

[Portfolio](https://nbit-51.github.io/portfolio/) · [GitHub](https://github.com/Nbit-51) · [Hugging Face](https://huggingface.co/Navaneeth123456789) · [LinkedIn](https://www.linkedin.com/in/navaneeth-singh-01930a2b4/)

---

## Current Focus

I’m currently exploring **inference-time efficiency** across both GPU and CPU architectures.

- **GPU inference:** Triton/CUDA kernels, kernel fusion, CUDA Graphs, quantization, speculative decoding
- **CPU inference:** C++ runtimes, AVX2 SIMD, memory locality, graph-level optimization
- **LLM systems research:** KV-cache compression, eviction strategies, quantized caches, architecture-specific behavior
- **Systems work:** ARMv8-A numerical computing, C++ performance engineering, WebAssembly

My broader goal is to work on **ML systems, inference runtimes, AI compilers, and hardware-efficient model deployment**.

---

## Featured Work

### [Hydra Engine](https://github.com/Nbit-51/Hydra_Engine)

A high-performance LLM inference project built around TinyLlama-1.1B.

The project explores fused Triton kernels, CUDA Graphs, speculative decoding, AVX2 token verification, NF4 quantization, LibTorch, and PyBind11.

Performance improvements are measured **per kernel and workload rather than represented as a single global speedup**, because the observed gains depend on execution conditions and the component being benchmarked.

**Tech:** C++17 · CUDA · Triton · PyTorch · LibTorch · PyBind11 · AVX2

---

### [Leaf](https://github.com/Nbit-51/Leaf)

A CPU-native neural-network inference optimization engine designed for machines without a GPU.

The current ResNet-18 path uses a compiled C++ runtime and a hand-tuned AVX2 GEMM implementation. In the current development setup, mean inference latency was reduced from **397.4 ms to 140.9 ms**, while the runtime output remained close to the PyTorch reference with a maximum absolute difference of **3.93e-06**.

Current directions include quantization, structured pruning, and transformer execution.

**Tech:** C++ · Python · ONNX · AVX2 · CMake · Quantization

---

### [KV Cache Compression Study](https://github.com/Nbit-51/LLM_MODELS_OPTIMIZATION_STUDY)

An ongoing empirical study of KV-cache optimization strategies across different LLM architectures.

The work compares approaches including:

- budget-based cache truncation
- H2O-style token eviction
- StreamingLLM
- INT4 / INT8 cache quantization
- sliding-window attention

The methodology has been evaluated on smaller variants across **OPT, IBM Granite, and Qwen2.5**, with current work focused on scaling the experiments and studying architecture-specific behavior.

**Tech:** Python · PyTorch · Transformers · Quantization · LLM Evaluation

---

## Other Engineering Work

### [navexa ARMv8-A Library](https://github.com/Nbit-51/navexa_ARMv8-A_Library)

Collaborative numerical-computing library for ARMv8-A. My contributions include the **SME Matrix Acceleration module** and **Virtualization Helpers**.

- Cross-compiled to AArch64 using CMake
- **109 / 109 tests passing**

### [LPG Distribution System](https://github.com/Nbit-51/LPG-Distribution-System)

A priority-aware LPG allocation platform designed to handle shortages more intelligently than simple first-come-first-served allocation.

Built with **FastAPI, MySQL, Python, REST APIs, allocation logic, and QR-based consumer tracking**.

This project won **1st place in a college datathon**.

### [ECS Component System](https://github.com/Nbit-51/Ecs_Component_System)

A C++ Entity Component System using contiguous storage and sparse sets to study cache-friendly data layouts and low-overhead iteration.

### [Math Relation Analyser](https://github.com/Nbit-51/Math-Relation-Analyser)

An interactive discrete-mathematics relation analyser with a C++ backend compiled to **WebAssembly** for in-browser execution.

### [ML Training Algorithms](https://github.com/Nbit-51/ML_Algorithms)

Implementations of neural-network training components created to study backpropagation, optimization algorithms, and model internals beyond framework-level abstractions.

---

## Technical Areas

**Machine Learning / Inference**

`PyTorch` · `Transformers` · `Triton` · `CUDA Graphs` · `Quantization` · `KV Cache` · `Speculative Decoding`

**Systems / Performance**

`C++17` · `CUDA` · `LibTorch` · `PyBind11` · `AVX2 SIMD` · `ARMv8-A` · `CMake` · `Linux`

**Backend / Tooling**

`Python` · `FastAPI` · `MySQL` · `REST APIs` · `JavaScript` · `HTML/CSS` · `Git`

---

## What I’m Trying to Understand

A recurring question behind most of my projects is:

> **Where does inference time actually go, and what changes when we stop treating the hardware as a black box?**

That question has taken me from model-level optimization into kernel fusion, cache behavior, SIMD, memory bandwidth, execution graphs, quantization, and KV-cache research.

I’m especially interested in work where **machine learning meets systems engineering**.

---

## Connect

I’m open to conversations around **ML systems, LLM inference, performance engineering, research collaborations, and internships**.

- **Portfolio:** [nbit-51.github.io/portfolio](https://nbit-51.github.io/portfolio/)
- **LinkedIn:** [Navaneeth Singh](https://www.linkedin.com/in/navaneeth-singh-01930a2b4/)
- **Hugging Face:** [Navaneeth123456789](https://huggingface.co/Navaneeth123456789)
- **Email:** navaneethsingh73@gmail.com
