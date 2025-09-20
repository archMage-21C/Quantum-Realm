---
tags:
date-created: 2025-09-03T20:02
last-updated: 2025-09-03T20:03
---
# :LiList: Table of Contents
---



# Topic Header
---
### The Core Idea: Simplifying Ray Tracing

Matrix optics provides a concise, algebraic method for tracking light rays through an optical system. Instead of using complex geometry and trigonometry to trace the path of a ray through lenses, mirrors, and free space, we can represent each optical component by a 2×2 matrix. The effect of a system of multiple components is then found by simply multiplying their individual matrices together.

This method is based on the **paraxial approximation**, which assumes that all rays are close to the optical axis and travel at small angles relative to it. Under this assumption, the sines and tangents of these angles can be approximated by the angles themselves (sinα≈tanα≈α).

### The Ray Vector and Ray Transfer Matrix

A light ray at a specific plane in an optical system is fully described by two parameters: its radial distance from the optical axis (r) and its angle with the optical axis (α). We combine these into a two-element **ray vector**:

$$ \mathbf{r} = \begin{pmatrix} r \ \alpha \end{pmatrix} $$

The effect of an optical component or a section of free space is to transform an incoming ray vector, r1​, into an outgoing ray vector, r2​. This transformation is linear and can be represented by a **ray transfer matrix**, M, also known as the ABCD matrix:

$$ \mathbf{r}_2 = \mathbf{M} \mathbf{r}_1 \implies \begin{pmatrix} r_2 \ \alpha_2 \end{pmatrix} = \begin{pmatrix} A & B \ C & D \end{pmatrix} \begin{pmatrix} r_1 \ \alpha_1 \end{pmatrix} $$

Each element of the ABCD matrix has a specific physical meaning:

- A=r1​r2​​ (when α1​=0): This relates the output height to the input height for a ray entering parallel to the axis. It is related to the system's magnification.
    
- B=α1​r2​​ (when r1​=0): This relates the output height to the input angle for a ray entering on the axis. It represents a measure of the system's focusing or collimating power.
    
- C=r1​α2​​ (when α1​=0): This relates the output angle to the input height for a ray entering parallel to the axis. It is related to the system's focal power (C=−1/f, where f is the effective focal length).
    
- D=α1​α2​​ (when r1​=0): This relates the output angle to the input angle for a ray entering on the axis.
    

The determinant of a ray transfer matrix for a system in a uniform medium is always unity: det(M)=AD−BC=1. This property is a consequence of Lagrange's invariant and holds for any system of passive components in a single medium.

### Ray Transfer Matrices for Common Optical Components

Here are the matrices for the most common elements in a simple optical system:

1. **Propagation through Free Space (or a uniform medium):** For a ray traveling a distance d in a medium with refractive index n (for air, n=1), the matrix is: $$ \mathbf{M}_{\text{space}} = \begin{pmatrix} 1 & d \ 0 & 1 \end{pmatrix} $$
    
2. **Thin Lens:** A thin lens of focal length f is represented by the matrix: $$ \mathbf{M}_{\text{lens}} = \begin{pmatrix} 1 & 0 \ -1/f & 1 \end{pmatrix} $$
    
3. **Spherical Mirror:** For a concave mirror with a radius of curvature R (R>0), the matrix is: $$ \mathbf{M}_{\text{mirror}} = \begin{pmatrix} 1 & 0 \ -2/R & 1 \end{pmatrix} $$ For a convex mirror, R is negative. This matrix represents the effect of the reflection at the mirror's surface.
    

### Cascading Optical Components

The true power of this method lies in its ability to handle complex systems. To find the total matrix for a series of components, we simply multiply their individual matrices in reverse order of how the light encounters them. For a system with N components, the total matrix Mtotal​ is:

$$ \mathbf{M}_{\text{total}} = \mathbf{M}_N \cdots \mathbf{M}_2 \mathbf{M}_1 $$

For example, a system consisting of a thin lens (focal length f1​) followed by free space (distance d) and then another thin lens (focal length f2​) would have the total matrix: $$ \mathbf{M}_{\text{total}} = \begin{pmatrix} 1 & 0 \ -1/f_2 & 1 \end{pmatrix} \begin{pmatrix} 1 & d \ 0 & 1 \end{pmatrix} \begin{pmatrix} 1 & 0 \ -1/f_1 & 1 \end{pmatrix} $$

This is a powerful method for designing and analyzing a wide range of optical instruments, from telescopes to laser cavities.


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