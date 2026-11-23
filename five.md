It looks like you accidentally sent the exact same prompt again! Since we just walked through the 4-particle square example for Steps 1 and 3, let's immediately apply those exact same steps to 5 particles (the pentagon) so you can see how the method scales up to multiple propagators and a 2D polytope.

Step 1: 5-Particle Relativistic Kinematics

Now imagine 5 massless scalar particles colliding in cyclic order \((1, 2, 3, 4, 5)\). Momentum conservation is:
\(p_{1}^{\mu }+p_{2}^{\mu }+p_{3}^{\mu }+p_{4}^{\mu }+p_{5}^{\mu }=0,\quad \text{with\ }p_{i}^{2}=0\)
In planar \(\text{Tr}(\phi^3)\) theory, each Feynman diagram for 5 external particles must have 3 cubic vertices and 2 internal propagators. There are exactly 5 planar diagrams, corresponding to the 5 cyclic rotations of pairing adjacent particles:
\(\mathcal{A}_{5}=\frac{1}{s_{12}s_{34}}+\frac{1}{s_{23}s_{45}}+\frac{1}{s_{34}s_{51}}+\frac{1}{s_{45}s_{12}}+\frac{1}{s_{51}s_{23}}\)
(where \(s_{ij} = (p_i + p_j)^2\)).

Step 3: Surfaceology on a Pentagon

Instead of drawing Feynman diagrams, draw a pentagon with vertices labeled 1, 2, 3, 4, 5 in cyclic order.

1. Map Chords to Planar Variables (\(X_{i,j}\))

As before, each boundary edge \((i, i+1)\) carries momentum \(p_{i}\). An internal chord connecting non-adjacent vertices \(i\) and \(j\) carries the sum of the momenta along one side of the cut:
• Chord \((1,3)\): Cuts off edges \(p_1, p_2 \implies X_{1,3} = (p_1 + p_2)^2 = s_{12}\)
• Chord \((2,4)\): Cuts off edges \(p_2, p_3 \implies X_{2,4} = (p_2 + p_3)^2 = s_{23}\)
• Chord \((3,5)\): Cuts off edges \(p_3, p_4 \implies X_{3,5} = (p_3 + p_4)^2 = s_{34}\)
• Chord \((1,4)\): Cuts off edges \(p_4, p_5 \implies X_{1,4} = (p_4 + p_5)^2 = s_{45}\)
• Chord \((2,5)\): Cuts off edges \(p_5, p_1 \implies X_{2,5} = (p_5 + p_1)^2 = s_{51}\)
Notice that every internal chord on the pentagon corresponds one-to-one with one of the 5 Mandelstam invariants!

2. Triangulate the Pentagon

To slice a pentagon into 3 triangles, you need 2 non-crossing internal chords. Every valid pair of non-crossing chords gives you one Feynman diagram:

Triangulation (Non-Crossing Chords)	Inverse Chord Product \(\frac{1}{X_{a,b}X_{c,d}}\)	Matching Feynman Diagram
Chords \((1,3)\) and \((1,4)\)	\(\frac{1}{X_{1,3}X_{1,4}}\)	\(\frac{1}{s_{12}s_{45}}\)
Chords \((1,3)\) and \((3,5)\)	\(\frac{1}{X_{1,3}X_{3,5}}\)	\(\frac{1}{s_{12}s_{34}}\)
Chords \((2,4)\) and \((2,5)\)	\(\frac{1}{X_{2,4}X_{2,5}}\)	\(\frac{1}{s_{23}s_{51}}\)
Chords \((2,4)\) and \((1,4)\)	\(\frac{1}{X_{2,4}X_{1,4}}\)	\(\frac{1}{s_{23}s_{45}}\)
Chords \((2,5)\) and \((3,5)\)	\(\frac{1}{X_{2,5}X_{3,5}}\)	\(\frac{1}{s_{51}s_{34}}\)


3. Build the 2D Associahedron

Each of the 5 triangulations becomes a vertex of a 2D shape. Two vertices are connected by an edge if you can get from one triangulation to the other by "flipping" (mutating) a single chord inside a quadrilateral sub-region:
• Start at \(\{(1,3), (1,4)\}\). Flip \((1,4) \to (3,5)\) to reach \(\{(1,3), (3,5)\}\).
• From \(\{(1,3), (3,5)\}\), flip \((1,3) \to (2,5)\) to reach \(\{(2,5), (3,5)\}\).
• Continue flipping one chord at a time—after 5 steps, you loop right back to where you started!
This traces out a 2D pentagon (the 2D associahedron \(K_{4}\)), whose 5 corners encode the 5 Feynman diagrams, and whose 5 edges represent the 5 internal propagators \(X_{i,j} = 0\).
Now that you've seen how polygons give tree-level diagrams, where would you like to go next?
Step 2 (Scalar QFT): Walk through how to actually derive the propagator \(\frac{1}{p^{2}}\) from a quantum field theory Lagrangian so you know where the physics rules come from.Beyond Polygons (Loops & Curves): See how adding a puncture (hole) in the middle of the disk turns this into a 1-loop scattering calculation using surfaceology's \(u\)-variables.
