Here is how you go from special relativity straight to your first surfaceology calculation for a 4-particle scattering process.

Part 1: Relativistic Kinematics (The Physics Setup)

Imagine 4 massless scalar particles colliding. In modern amplitudes, we treat all particles as incoming, so four-momentum conservation is:
\(p_{1}^{\mu }+p_{2}^{\mu }+p_{3}^{\mu }+p_{4}^{\mu }=0\)
Because the particles are massless, each four-momentum squares to zero:
\(p_{i}^{2}=p_{i}^{\mu }p_{i\mu }=0\)
We define the Mandelstam variables to capture the Lorentz-invariant combinations of momenta:
• \(s = (p_1 + p_2)^2 = 2(p_1 \cdot p_2)\)
• \(t = (p_2 + p_3)^2 = 2(p_2 \cdot p_3)\)
• \(u = (p_1 + p_3)^2 = 2(p_1 \cdot p_3)\)
(Note: Using momentum conservation \(p_1 + p_2 = -(p_3 + p_4)\), you can check that \(s = (p_3 + p_4)^2\) and \(t = (p_1 + p_4)^2\).)
In planar \(\text{Tr}(\phi^3)\) theory, the particles have a fixed cyclic order around a circle: \((1, 2, 3, 4)\). Because of this ordering, the \(u\)-channel (which crosses lines 1 and 3 over 2 and 4) is non-planar and drops out. The total tree-level planar amplitude is simply the sum of the two planar Feynman diagrams:
\(\mathcal{A}_{4}=\frac{1}{s}+\frac{1}{t}\)

Part 2: Surfaceology (Turning Diagrams into a Square)

Now forget Feynman diagrams and spacetime. Follow the surfaceology recipe for \(n = 4\) particles:

1. Draw the Surface

Draw a disk and place \(4\) marked points on its boundary in cyclic order: 1, 2, 3, 4. Connect the boundary points with straight edges to form a square (a 4-gon).

2. Map Chords to Kinematics (\(X_{i,j}\))

Instead of labeling edges with momenta \(p_{i}\), label the vertices of the square \(1, 2, 3, 4\) such that the boundary edge between vertex \(i\) and vertex \(i+1\) carries momentum \(p_{i}\):
• Edge \((1,2)\) carries \(p_{1}\)
• Edge \((2,3)\) carries \(p_{2}\)
• Edge \((3,4)\) carries \(p_{3}\)
• Edge \((4,1)\) carries \(p_{4}\)
Any internal chord connecting vertex \(i\) to vertex \(j\) cuts the square in two. By momentum conservation, the momentum flowing across that chord is the sum of the boundary edges on one side of it. We define the planar variable \(X_{i,j}\) as the square of that momentum:
• Chord \((1,3)\): Separates edges \(p_1, p_2\) from \(p_3, p_4\). Therefore:
\(X_{1,3}=(p_{1}+p_{2})^{2}=s\)
• Chord \((2,4)\): Separates edges \(p_2, p_3\) from \(p_4, p_1\). Therefore:
\(X_{2,4}=(p_{2}+p_{3})^{2}=t\)

3. Triangulate the Square

A cubic Feynman diagram (where 3 lines meet at every vertex) is the dual graph of a triangle. Therefore, slicing our square into triangles using non-crossing internal chords gives every possible planar Feynman diagram:
• Triangulation A: Draw chord \((1,3)\). This slices the square into two triangles: \((1,2,3)\) and \((1,3,4)\). Assigning \(1/X_{i,j}\) to each internal chord gives the amplitude \(\frac{1}{X_{1,3}} = \frac{1}{s}\).
• Triangulation B: Draw chord \((2,4)\). This slices the square into two triangles: \((2,3,4)\) and \((2,4,1)\). This gives the amplitude \(\frac{1}{X_{2,4}} = \frac{1}{t}\).
You cannot draw both chords at the same time because they cross in the middle of the square.

Part 3: The Associahedron (The Geometry)

How do we combine Triangulation A and Triangulation B into a single geometric object?
1. Vertices: Represent Triangulation A as a point on the left (\(x = 0\)) and Triangulation B as a point on the right (\(x = L\)).
2. Edge (Mutation): You transform Triangulation A into Triangulation B by deleting chord \((1,3)\) and inserting chord \((2,4)\). Connecting these two points creates a 1-dimensional line segment of length \(L = s + t\).
3. The Amplitude as Volume: In positive geometry, the scattering amplitude is the canonical form of this line segment—which for a 1D interval \([0, L]\) turns out to be proportional to the sum of the inverse distances to its two endpoints:
\(\Omega =\left(\frac{1}{x}+\frac{1}{L-x}\right)dx\)
Setting the distance to the left wall as \(x = X_{1,3} = s\) and the distance to the right wall as \(L - x = X_{2,4} = t\) (which fixes the total length of the line segment to \(L = s + t\)), the coefficient of the canonical form immediately gives the full quantum field theory amplitude:
\(\mathcal{A}_{4}=\frac{1}{X_{1,3}}+\frac{1}{X_{2,4}}=\frac{1}{s}+\frac{1}{t}\)

Summary Table: Physics vs. Surfaceology (\(n=4\))


Physics (Feynman Diagrams)	Surfaceology (Triangulated Square)
External particle momentum \(p_{i}\)	Boundary edge \((i, i+1)\) of the square
Momentum conservation \(\sum p_i = 0\)	Closed boundary of the polygon
Internal propagator \(\frac{1}{(p_{1}+p_{2})^{2}}\)	Internal diagonal chord \(\frac{1}{X_{1,3}}\)
Cubic interaction vertex	A single triangle inside the triangulation
Sum over all planar diagrams	Vertices of the 1D associahedron (line segment)

Ready to level up to 5 particles (a pentagon)? If you'd like, we can:
Count the 5 triangulations of a pentagon and see how they form a 2D associahedron (which is itself a pentagon!).Preview "curves and \(u\)-variables" to see how surfaceology replaces the sum over triangulations with a single smooth integral.
