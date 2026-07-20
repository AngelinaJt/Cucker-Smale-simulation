# Cucker-Smale Flocking Simulation

## Overview

This repository contains a numerical simulation of the classical **Cucker–Smale flocking model** in two dimensions.

The simulation is implemented in **Python** using **NumPy** and **Matplotlib**. The system is solved using the classical **fourth-order Runge–Kutta (RK4)** method and visualized through an animated velocity field.

This project was developed as part of a Master's research work in applied mathematics.

---

## Mathematical model

The Cucker–Smale system is defined by

```math
\dot{x}_i = v_i,
```

```math
\dot{v}_i =
\frac{\alpha}{N}
\sum_{j=1}^{N}
\phi(\|x_j-x_i\|)
\left(v_j-v_i\right),
```

where the communication kernel is defined by

```math
\phi(r)=\frac{1}{(1+r^2)^{\beta/2}}.
```
---

## Simulation parameters

| Parameter | Value |
|-----------|------:|
| Number of particles | 20 |
| Dimension | 2 |
| Final time | 10 |
| Time step | 0.05 |
| α | 1 |
| β | 0.5 |

---

## Contents

- `Cucker_Smale_Simulation.ipynb` : complete simulation notebook.
- Animated visualization of the particle system.
- RK4 numerical integration.

---

## Requirements

- Python 3
- NumPy
- Matplotlib

---

## Author

Angelina Jt

Master's research project in Applied Mathematics.
