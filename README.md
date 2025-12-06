# HyperCo
Hypersurface Co-design Framework for Structural Optimisation

# Co-design of Structures via Generalized Evolution

MATLAB Implementation of Liu et al., CMA 2025

This repository contains the MATLAB source code accompanying:

Liu, Y., Xia, B., Li, Z., Ren, H., Du, J., Tan, W. (2025).
Co-design of structures via generalized evolution.
Computer Methods in Applied Mechanics and Engineering, 118584.
https://doi.org/10.1016/j.cma.2025.118584

The framework enables simultaneous shape and topology optimisation by evolving two surrogate hypersurfaces through tangential (shape) and orthogonal (topology) evolution. A quasi-conformal transformation ensures compatibility, and an ALE method maintains mesh quality during structural evolution.

The method offers a unified mathematical framework for simultaneous shape and topology optimisation by evolving two surrogate hypersurfaces via tangential (shape) and orthogonal (topology) motions. A quasi-conformal transformation ensures consistent geometry updates, while an ALE strategy preserves mesh quality during evolution.

##  Impact

This framework enables structurally superior designs that cannot be achieved using shape or topology optimisation alone. By integrating both within a single evolution equation, the method:

Provides a general and flexible co-design strategy applicable to single-material and composite structures.

Produces higher-performance geometries with improved stiffness, load paths, and material efficiency.

Allows smooth transitions between shape change and topological change, avoiding mesh distortion and common failure modes of traditional methods.

Establishes a new foundation for next-generation structural optimisation, bridging mathematical rigor, mechanical interpretation, and practical implementation.

This unified approach expands the design space and enables engineers and researchers to explore truly co-designed structural solutions, opening doors to applications in aerospace, civil engineering, energy, and advanced manufacturing.

## Software Requirements

MATLAB R2020a or newer

No external toolboxes required

Examples and main solver run on standard installations

Recommended: machine with 16+ GB RAM for larger meshes

## How to Run the Code
Direct Run (Recommended)

Open MATLAB

Set the repository folder as your current working directory

Open the file from the folder. 

Click the green “Run” button

This will execute a default co-design example.

| **Optimisation Type**                             | **Evolution Manner(s)** | **Material System** |
| ------------------------------------------------- | ----------------------- | ------------------- |
| **Material optimisation**                         | **TEₓ_S**               | Single-material     |
|                                                   | **TEᵧ_S**               | Single-material     |
|                                                   | **TEₓᵧ_S**              | Single-material     |
| **Shape optimisation**                            | **OEₒ_S**               | Single-material     |
| **Topology optimisation**                         | **CEₓₒ_S**              | Single-material     |
|                                                   | **CEᵧₒ_S**              | Single-material     |
| **Collaborative optimisation** (shape + topology) | **CEₓᵧₒ_S**             | Single-material     |
| **Composite optimisation**                        | **OEₒ_C**               | Composite           |
|                                                   | **CEₓₒ_C**              | Composite           |
|                                                   | **CEᵧₒ_C**              | Composite           |
|                                                   | **CEₓᵧₒ_C**             | Composite           |


