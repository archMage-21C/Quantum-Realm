---
tags:
date-created: 2025-09-21T21:06
last-updated: 2025-09-21T23:49
---
# **The Wave Equation**
---
### <u>Derivation Using a Vibrating String Model</u>

Let's imagine a string with a uniform linear mass density $\mu$ (kg/m) under a constant tension $T$ N (Newtons). Let $u(x,t)$ be the small vertical displacement of the string at position $x$ and time $t$. We'll make two key assumptions for small vibrations:

- The displacement $u$ is small, so the angle $\theta$ the string makes with the horizontal is also small. This means we can approximate $sin(\theta) \approx tan(\theta) \approx \frac{\partial x}{\partial y}$ ​.  
- The tension $T$ is constant everywhere along the string.

Now, consider an infinitesimally small segment of the string between $x$ and $x+dx$, as shown below.

1. **Analyze the Forces:** The only forces acting on this segment are the tension forces from the left, $T_{1}$, and from the right, $T_{2}$ ​. The net vertical force, $F_{y}$ ​, is the sum of the vertical components of these tensions.
    - Vertical force from the right: $T_{2y}​=Tsin(\theta_{2}​) \approx Ttan (\theta_{2}​) = T(\frac{\partial u}{\partial x})|​_{x+dx}$.
    - Vertical force from the left: $T_{1y}​=-Tsin(\theta_{1}​) \approx -Ttan (\theta_{1}​) = -T(\frac{\partial u}{\partial x})|​_{x}$
    - The net vertical force is $F_{y}​= T_{1y} + T_{2y} = T\lbrack \frac{\partial u}{\partial x}|​_{x+dx} - \frac{\partial u}{\partial x}|​_{x} \rbrack$.
  
2. **Connect Force to Curvature:** The term in the brackets is the _change_ in the slope over the distance $dx$. From the definition of a second derivative, this change is precisely the curvature multiplied by $dx$.
    - $\frac{\partial u}{\partial x}|​_{x+dx} - \frac{\partial u}{\partial x}|​_{x}​ \approx \frac{\partial}{\partial x}(\frac{\partial u}{\partial x})​dx = \frac{\partial^2u}{\partial x^2}dx$.
    - So, the net force is directly proportional to the curvature: $F_{y}​=T\frac{\partial^2u}{\partial x^2}dx$.

3. **Apply Newton's Second Law:** The mass of our small segment is $m=\mu⋅dx$. Its vertical acceleration is $a_{y}​=\frac{\partial^2u}{\partial t^2}​$. According to Newton's law:
    - $F_{y}​=ma_{y}​=(\mu⋅dx)\frac{\partial^2u}{\partial t^2}​$.

4. **Form the Equation:** Now we equate our two expressions for the net force $F_{y}$ ​:
$$
T\frac{\partial^2u}{\partial x^2}dx = \mu\frac{\partial^2u}{\partial t^2}dx​
$$
    Dividing by $T⋅dx$ and rearranging gives us the 1D wave equation:
$$
\frac{\partial^2u}{\partial x^2}dx = \frac{\mu}{T}\frac{\partial^2u}{\partial t^2}
$$
    By comparing this to the standard form, we see that the wave speed is $c=\sqrt{\frac{T}{\mu}}​$. The speed depends only on the properties of the medium (tension and mass density).

##### **Generalization to 3D**

The physical reasoning is the same in three dimensions, but the math is slightly different. The curvature of the wave at a point is no longer described by a simple second derivative but by the **Laplacian operator**, $\nabla^2u = \frac{\partial^2u}{\partial x^2} + \frac{\partial^2u}{\partial y^2} + \frac{\partial^2u}{\partial z^2}$. Replacing the 1D curvature term with the 3D Laplacian gives us the general wave equation:

$$
\nabla^2u(r,t)−\frac{1}{c^2}\frac{\partial^2 u(r,t)}{\partial t^2}​=0
$$


This is the central equation of wave optics. It describes how any optical wave disturbance $u$ evolves in space and time as it propagates through a medium with wave speed $c$.
### <u>Key Concepts</u>
- Explanation of the key concepts of this topic.


# :LiListFilter: Highlights
---
### <u>Key Takeaways</u>
- Key takeaways from this note.

### <u>Important Dates</u>
- List of important dates (if applicable).

### <u>Formulas & Equations</u>
- List of important formulas (if applicable).

### <u>Graphs & Charts</u>
- List of important graphs (if applicable).