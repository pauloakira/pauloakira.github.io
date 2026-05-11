---
title: "POLI-VEM"
excerpt: "A C++17 library implementing the Virtual Element Method (VEM) and Finite Element Method (FEM) for structural analysis, with Python bindings and a FastAPI middleware."
collection: portfolio
date: 2024-12-01
---

POLI-VEM is my main research codebase — a C++17 library implementing the Virtual
Element Method (VEM) and Finite Element Method (FEM) for problems in solid
mechanics, with a `pybind11` Python interface and a FastAPI REST middleware.

**Solvers implemented**

- **1D Euler-Bernoulli beam VEM** — arbitrary-order solver with static condensation
  and distributed-load assembly.
- **2D linear elastic VEM (k ≥ 1)** — energy projection $\Pi^\nabla$ for $k=1$ and
  L²-strain projection $\Pi^\varepsilon$ for $k \geq 1$ (Artioli et al. 2018), with
  verified convergence rates $O(h^k)$ on Voronoi and distorted polygonal meshes
  ($k = 1, 2, 3$).
- **2D axisymmetric VEM** — rotational-symmetry formulation incorporating the radial
  weight in the weak form; supports `standard`, `divergence`, and `boundary`
  stabilization strategies.
- **Parabolic VEM** — time-dependent heat conduction with multiple time-integration
  schemes.
- **2D nonlinear VEM** — finite-deformation hyperelasticity with a Neo-Hookean
  energy and two stabilization families:
  - *Coupled (Van Huyssteen)* — triangulation-based, autodiff tangent, modified
    Lamé parameters to prevent volumetric locking.
  - *Decoupled (kernel-based)* — submesh-free, constant precomputed tangent,
    deviatoric/volumetric decomposition in the principal frame.
- **Hyperelastic FEM reference** — Q1, Q8 (2D) and H8 (3D) elements, Newton solver,
  benchmarked against Cook's membrane.

**Stack**

C++17 · Eigen3 · nlohmann/json · OpenCV · autodiff · pybind11 · FastAPI.
JSON mesh format, manufactured-solution convergence harnesses, Cook's-membrane
benchmarks for k = 1, 2, 3.

This codebase backs several of the papers on the [Publications](/publications/)
page (axisymmetric VEM, parabolic VEM with SSP-RK time stepping, finite-strain
stabilization scaling, and the hybrid VEM + deep-learning Euler-Bernoulli work).
