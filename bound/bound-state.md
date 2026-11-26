A master’s thesis in numerical/computational bound-state QED works best when it targets a self-contained, computationally tractable formalism rather than full multi-loop diagram resummation. Three concrete, well-scoped thesis problems align directly with these constraints:

1. Basis Light-Front Quantization (BLFQ) for Positronium or Muonium

In light-front QFT, bound states are obtained by diagonalizing a large sparse Hamiltonian matrix in a discretized Fock-space basis. While positronium has been studied in low Fock sectors (\(\vert{}e^+e^-\rangle + \vert{}e^+e^-\gamma\rangle\)), extending accuracy and handling renormalization remains active.
• The Problem: Implement a BLFQ solver to compute the mass spectrum, hyperfine splitting, and electromagnetic form factors of positronium (or unequal-mass muonium) at strong or physical coupling α. Investigate how sector-dependent mass counterterms and basis truncation cutoffs (\(N_{\max }\), K) affect rotational symmetry restoration across different magnetic projections (\(m_J = 0, \pm 1\)).
• Computational Core: Constructing sparse Hamiltonian matrices using harmonic oscillator basis functions, solving large-scale eigenvalue problems (Lanczos/Arnoldi algorithms in Python, Julia, or C++), and performing basis-cutoff extrapolations.
• Why It Fits a Master's: The theoretical formalism is well-established by groups like Vary, Li, and Wiecki, allowing you to start with a working 2-Fock-sector benchmark and push into unequal masses, higher Fock sectors, or light-front wave function observables.

2. Minkowski-Space Bethe–Salpeter Equation (BSE) via Nakanishi Representation

Standard Bethe–Salpeter solvers rely on Wick rotation to Euclidean space, which breaks down when calculating time-like form factors or parton distributions. Solving the BSE directly in Minkowski space avoids this bottleneck.
• The Problem: Solve the fermionic Bethe–Salpeter equation for positronium in the ladder approximation directly in Minkowski space by projecting onto the Nakanishi integral representation (NIR). Compare the resulting bound-state masses and light-front projections against Euclidean BSE and non-relativistic Schrödinger benchmarks across a range of couplings.
• Computational Core: Converting singular integral equations into smooth, non-singular generalized eigenvalue problems using orthogonal polynomials (Gegenbauer/Laguerre) and Gauss quadrature.
• Why It Fits a Master's: Unlike lattice or large-scale Fock space diagonalization, Nakanishi-based Minkowski solvers run quickly on a single workstation, leaving plenty of room to explore gauge dependence (Feynman vs. Landau gauge) or crossed-ladder kernel corrections.

3. Strong-Field QED Bound States & Vacuum Polarization (Supercritical Zα → 1)

When a nuclear charge Z approaches the critical threshold (Zα ≈ 1, such as in heavy-ion collisions or superheavy elements), perturbation theory in Zα breaks down completely as the \(1s_{1/2}\) state dives into the negative-energy Dirac continuum.
• The Problem: Numerically compute the bound-state energy levels and exact one-loop vacuum polarization (Uehling and Wichmann–Kroll potentials) for a Dirac electron in a finite-size nuclear potential as Zα → 1. Track the behavior of the bound state and induced vacuum charge density near the supercritical diving threshold.
• Computational Core: Solving coupled radial Dirac differential equations with finite-difference or B-spline basis methods, combined with partial-wave Green's function summations for the Wichmann–Kroll term.
• Why It Fits a Master's: It connects fundamental non-perturbative QED physics (vacuum instability and pair creation) to clean numerical linear algebra and differential equation solvers without requiring heavy high-performance computing clusters.

Recommended Next Step

If you want to evaluate one of these for a thesis proposal, Basis Light-Front Quantization (Option 1) is often the easiest to scale up incrementally—you can reproduce known results within a few weeks and then vary parameters (coupling strength, mass ratio, or basis truncation) for original results.
If you let me know:
• Your primary programming language (e.g., Python, C++, Julia, Fortran)
• Your timeline (e.g., 6 months vs. 1 year)
• Whether you have a local advisor working in light-front, covariant, or atomic QED
I can help draft a concrete project outline with starting equations and benchmark papers.
