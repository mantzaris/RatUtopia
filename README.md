# Rat Utopia — Uncertainty-Driven Agent-Based Model

This repository contains Julia code for simulating Calhoun's Universe-25 using two complementary approaches:

- **Game-matrix surrogate** that reproduces the same macro patterns using a population-level engagement variable.
- **Agent-Based Model (ABM)** built with [`Agents.jl`](https://juliadynamics.github.io/Agents.jl/stable/), where each rat has sex, age, rank, engagement propensity, and survival dynamics driven by a time-varying **uncertainty** schedule.


The core hypothesis is that as social hierarchy becomes more 'visible' (lower uncertainty), engagement collapses, reducing reproduction and accelerating decline—producing the observed growth -> plateau -> extinction arc.

---

## Requirements

- Julia >= 1.9
- Packages: `Agents`, `Distributions`, `DataFrames`, `Plots`, `Statistics`, `Measures`, `Random`  
  *(optional for the matrix model: `CSV`)*

Install from the Julia REPL:
```julia
using Pkg
Pkg.activate(".")
Pkg.instantiate()
```