---
title: "GRAD-TUNING"
excerpt: "An ARM64-optimised deep-learning framework: a C++ tensor library using BLAS + SLEEF + NEON SIMD, exposed to Python, building up toward autodiff, transformers, and small language models."
collection: portfolio
date: 2024-08-01
---

A deep-learning framework optimized for ARM64 processors. The goal is a numerical
library focused on high performance and computational efficiency for both research
prototyping and production inference, built from the metal up rather than wrapping
an existing framework.

**Tensor core (built)**

A C++ tensor library with a Python binding layer (`core.tensor`, `core.nn`):

- Linear-algebra operations — matmul, batched matmul, elementwise add/sub/mul,
  scalar multiplication, dot product.
- Tensor views — transpose, reshape, contiguity checks.
- Activation functions implemented with **SLEEF** (vector-math libraries) and
  **NEON** (ARM SIMD intrinsics): ReLU, Sigmoid, tanh.
- Direct integration with BLAS for the heavy linear-algebra kernels.
- Streamlined memory management aimed at avoiding unnecessary copies.

**Roadmap (in progress)**

Reverse-mode automatic differentiation, gradient accumulation, the full
backpropagation pipeline, SGD and Adam optimizers, multithreading and GPU
back-ends. The downstream goal is full transformer-class workloads —
self-attention, multi-head attention, transformer blocks, and ultimately small
language models — running on an efficient, dependency-light ARM64 stack.

**Motivation**

Apple-silicon and ARM-server machines are now the default for many ML workloads,
but most deep-learning libraries are still tuned primarily for x86 / CUDA. GRAD-TUNING
is an experiment in what a "first-principles" deep-learning stack looks like when
the ARM64 vector unit, BLAS, and SLEEF are first-class targets from day one.
