To master the prerequisites for surfaceology, focus on a targeted subset of graduate physics and modern combinatorics rather than attempting to learn every subfield exhaustively.
You can break your preparation down into three specific tracks:

1. Quantum Field Theory (QFT) & Amplitudes

You do not need deep expertise in the Standard Model or condensed matter QFT. Instead, focus on the modern "on-shell" scattering amplitudes program:

• Scalar \(\text{Tr}(\phi^3)\) Theory: Learn how colored (matrix-valued) scalar particles interact via cubic vertices and how large-\(N\) color ordering organizes Feynman diagrams into planar and non-planar topologies.

• Kinematics & Mandelstam Variables: Get comfortable expressing scattering amplitudes purely in terms of Lorentz-invariant dot products of external momenta (\(p_i \cdot p_j\)) and planar variables (\(X_{i,j}\)).

• Tree vs. Loop Integrands: Understand the difference between a tree-level amplitude (rational functions of momenta) and a loop-level integrand (before performing the actual spacetime loop integration).

• Where to learn: Scattering Amplitudes in Gauge Theory and Gravity by Henriette Elvang and Yu-tin Huang  PDF on arXiv https://arxiv.org/abs/1308.1697 (specifically the introductory chapters on color ordering and kinematics). See also [](Scattering.md)

2. Combinatorics & Positive Geometry

Surfaceology translates physics into discrete shapes and piecewise-linear math. Focus on these specific geometric objects:
• The Associahedron: Study how triangulations of an \(n\)-gon correspond to the vertices of a convex polytope, and how flipping a diagonal corresponds to  moving along an edge.
• Canonical Forms: Learn the defining property of a "positive geometry"—a differential form whose logarithmic singularities lie exclusively on the boundaries of the shape.
• Tropical Geometry (Crucial): Surfaceology relies heavily on tropicalizing integrals. You should understand how to replace standard addition and multiplication with "max" and "plus" operations (\(a \oplus b = \max(a,b)\) and \(a \otimes b = a + b\)) to turn smooth spaces into piecewise-linear fans.
• Where to learn: Lectures on "Positive Geometries" by Thomas Lam or Nima Arkani-Hamed, and Introduction to Tropical Geometry by Diane Maclagan and Bernd Sturmfels (Chapter 1–2).

https://www.cambridge.org/core/books/scattering-amplitudes-in-gauge-theory-and-gravity/34C045B8331E6FF229E2496F6D8321C5 

https://arxiv.org/abs/1308.1697 Scattering Amplitudes
Henriette Elvang, Yu-tin Huang

https://janos.cs.technion.ac.il/COURSES/238900-13/Tropical/MaclaganSturmfels.pdf 

3. Topology & Cluster Algebras

To handle loop-level physics, surfaceology moves from simple polygons to punctured surfaces with handles:
• Riemann Surfaces & Triangulations: Understand 2D surfaces defined by their genus \(g\) (holes/handles) and boundary components with marked points. You will need to understand mapping class groups (how curves wind around punctures and handles infinitely many times).
• Cluster Algebras (Basic): Learn how "mutations" transform one triangulation into another and how algebraic variables (\(u\)-variables) are assigned to curves on a surface so that they satisfy specific polynomial identities.

• Where to learn: Cluster Algebras and Triangulated Surfaces by Sergey Fomin, Michael Shapiro, and Dylan Thurston (a very readable, foundational paper).

https://arxiv.org/abs/math/0608367

Summary Study Order

 an introduction to the theory of algebraic varieties emphasizing the
similarities to the theory of manifolds. https://www.jmilne.org/math/CourseNotes/AG.pdf 

Priority	Subject	Core Concept to Master

1	Planar QFT	Color-ordered \(\text{Tr}(\phi^3)\) diagrams & planar variables \(X_{i,j}\)

2	Polytopes	Polygon triangulations & the associahedron

3	Tropical Math	Piecewise-linear fans & tropicalizing functions

4	Surface Topology	Punctured surfaces, winding curves, & cluster mutations

