---
tags:
  - optics
  - wave-optics
date-created: 2025-09-21T22:39
last-updated: 2025-09-21T23:44
---
# **Postulates of wave optics**
---
```ad-tip
title: My Intuition
At its core, wave optics (also known as scalar wave optics) treats light as a wave, but simplifies things by describing it with a single scalar function—the **wavefunction**, usually denoted as u(r,t). Think of this as a simplified representation compared to the full vector electric and magnetic fields in electromagnetic theory. This scalar wave still captures the essential wavelike behaviors of light, such as propagation, interference, and diffraction, which ray optics cannot explain. The theory is built on two key ideas: how this wave travels and how we connect it to a measurable quantity, its intensity.
```

Wave optics is founded on two fundamental postulates that describe the behavior and measurement of light as a scalar wave.
### <u>1. The Wave Equation</u>

The first postulate states that light propagates as a wave described by a wave function, $u(r,t)$, which is a real function of position $r$ and time $t$. In a source-free, homogeneous, and isotropic medium, this wave function must satisfy the **wave equation**:
$$
\nabla^2u(r,t)−\frac{1}{c^2}\frac{\partial^2 u(r,t)}{\partial t^2}​=0
$$
Where the terms:

- $\nabla^2$ is the Laplacian operator, which describes the spatial variation of the wave.
- $c$ is the speed of light in the medium. For a medium with refractive index $n$, this speed is $c=\frac{c_{0}}{n}​$, where $c_{0}$ ​ is the speed of light in a vacuum.

A crucial consequence of this postulate is the **principle of superposition**. Since the wave equation is linear, if $u_{1}$ ​and $u_{2}​$ are valid solutions, then their sum $u_{1}+u_{2}​$ is also a valid solution. This is the mathematical foundation for the phenomenon of interference.

### <u>2. Optical Intensity</u>

The second postulate connects the abstract wave function to a physically measurable quantity: the **optical intensity**, $I(r,t)$. The intensity, which represents optical power per unit area, is proportional to the time average of the square of the wave function:
$$
I(r,t)=2⟨u2(r,t)⟩
$$
The angle brackets $⟨⋅⟩$ signify a time average over a duration that is much longer than a single optical cycle (which is on the order of femtoseconds) but shorter than any other timescale of interest (like the duration of a light pulse). This postulate allows us to predict the patterns of light and dark that we can actually observe and measure in experiments, such as interference fringes.

These two postulates form the bedrock of wave optics and provide a powerful framework for understanding a vast range of optical phenomena.