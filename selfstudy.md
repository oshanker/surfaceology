For self-studying your way up to Scattering Amplitudes in Gauge Theory and Gravity and surfaceology, follow a streamlined, bottom-up curriculum that skips traditional QFT detours (like canonical quantization or renormalization) and focuses strictly on kinematics, scalar Feynman rules, and discrete geometry.

Phase 1: Math & Relativity Foundations

Before touching field theory, make sure you can manipulate four-vectors and basic topology fluently:
• Special Relativity & Four-Vectors: Master index notation (\(p^{\mu }p_{\mu }\)), metric signatures, and Mandelstam invariants (\(s, t, u\)).
	• Resource: David Tong’s Dynamics and Relativity lecture notes (available free online; read the final chapter on Special Relativity).
• Elementary Topology & Graphs: Learn Euler’s polyhedron formula (\(V - E + F = 2 - 2g\)), dual graphs, and how triangulations of polygons relate to planar trees.
	• Resource: 3Blue1Brown’s videos on Euler's formula or introductory chapters of Stillwell’s Classical Topology and Combinatorial Group Theory.

Phase 2: Minimalist Quantum Field Theory

Skip heavy textbooks like Peskin & Schroeder at first. You only need to know how to write down a scalar amplitude from a Feynman diagram:
• Scalar \(\phi ^{3}\) Feynman Rules: Learn how propagators (\(1/p^2\)) and cubic vertices work in momentum space without spinor indices or gauge fixing.
	• Resource: David Tong’s Quantum Field Theory lecture notes (free online; read Chapters 1–3, stopping right after scalar Feynman diagrams).

https://davidtong.org/teaching/quantum-field-theory/

https://davidtong.org/pdfs/teaching/quantum-field-theory/qft.pdf 
	
• Alternative Book: Tom Lancaster & Stephen Blundell’s Quantum Field Theory for the Gifted Amateur (specifically written for self-learners; read Chapters 1–18).

https://dn721505.ca.archive.org/0/items/quantum-field-theory-for-the-gifted-amateur-blundell/Quantum-Field-Theory-For-The-Gifted-Amateur%20-%20Blundell.pdf

• Matrix/Color Ordering: Learn how \(N \times N\) matrix fields turn Feynman diagrams into ribbon graphs (double-line notation) that live naturally on 2D surfaces.

• Resource: Anthony Zee’s Quantum Field Theory in a Nutshell (Chapter VII.4 on the Large \(N\) Expansion).

https://people.stat.ucla.edu/ywu/Zee.pdf 

Phase 3: Bridge to On-Shell Amplitudes & Polytopes

Once you can compute a 4-particle scalar scattering amplitude by hand, transition directly into modern geometric methods:
• Video Lectures (Best for Self-Study): Watch Johannes Henn’s or Henriette Elvang’s TASI lectures on Scattering Amplitudes on YouTube alongside the Elvang & Huang textbook 

https://www.cambridge.org/core/books/scattering-amplitudes-in-gauge-theory-and-gravity/34C045B8331E6FF229E2496F6D8321C5 

to see calculations worked out line-by-line.
• Hands-On Practice: Draw a pentagon, find all 5 of its triangulations, and match each triangulation to a 5-particle tree-level Feynman diagram—this single exercise bridges Phase 2 directly into surfaceology.

Self-Study Roadmap Summary


Stage	Goal	Best Free / Self-Study Resource
1. Kinematics	Compute \(s, t, u\) invariants	David Tong’s Relativity notes
2. Feynman Rules	Calculate scalar \(\phi ^{3}\) tree diagrams	Tong’s QFT notes (Ch. 1–3) or QFT for the Gifted Amateur
3. Color & Surfaces	Use double-line notation for matrix fields	Zee’s QFT in a Nutshell (Large-\(N\) chapter)
4. Polytopes	Map diagrams to associahedra	Elvang & Huang (Ch. 1–3, 10) + TASI YouTube lectures




Having special relativity and basic quantum mechanics puts you in a great spot. You already have the hardest conceptual prerequisites out of the way and can skip straight to building your QFT toolkit and jumping into geometry.
Follow this focused, three-step action plan to get from your current background to surfaceology:

Step 1: Build Relativistic Kinematics Fluency (1–2 Weeks)

Before touching quantum fields, make sure you can do relativistic particle collision math in your sleep.
• What to learn: Four-momentum conservation (\(\sum p_i^\mu = 0\), using the all-incoming convention), dot products (\(p_i \cdot p_j\)), and Mandelstam variables (\(s = (p_1+p_2)^2\), \(t = (p_1+p_3)^2\), \(u = (p_1+p_4)^2\)).
• Action item: Verify for yourself that for 4 massless particles (\(p_i^2 = 0\)), \(s + t + u = 0\). Surfaceology relies heavily on rewriting these invariants in terms of "planar variables" \(X_{i,j} = (p_i + p_{i+1} + \dots + p_{j-1})^2\).

Step 2: Learn Minimalist Scalar Feynman Rules (2–4 Weeks)

You do not need a full year-long QFT course. You only need to understand how classical fields become quantum particles and how to read a diagram.
• Resource: Read Chapters 1–3 of David Tong’s Quantum Field Theory lecture notes (free online) or Chapters 1–18 of Quantum Field Theory for the Gifted Amateur.
• What to focus on:
	• Second quantization (turning harmonic oscillators into creation/annihilation operators \(a_p^\dagger, a_p\)).
	• The Feynman propagator (\(i/(p^2 - m^2 + i\epsilon)\)) and cubic interaction vertices (\(-ig\)).
	• Writing down a tree-level scattering amplitude directly from a diagram in momentum space.

Step 3: Connect Diagrams to Polygons (1 Week)

Once you can write down a basic \(\phi ^{3}\) Feynman diagram, you are ready for your first surfaceology calculation.
• Resource: Read Chapter 2 (Color Ordering) and Chapter 10 (Polytopes) of Elvang & Huang’s Scattering Amplitudes alongside Giulio Salvatori’s interactive visualizer (Surfaceology, by scrolling).
• The Milestone Exercise: Take a 4-particle planar scattering process (particles 1, 2, 3, 4 arranged around a square).
	1. Draw the two diagonal chords of the square: chord \((1,3)\) and chord \((2,4)\).
	2. Notice that each triangulation of the square corresponds to one of the two planar Feynman diagrams (the \(s\)-channel \(1/s\) and the \(t\)-channel \(1/t\)).
	3. Because you cannot draw both chords at once without crossing them, the two diagrams form the two endpoints of a 1D line segment—the simplest associahedron.

Your Next 30 Days at a Glance


Week	Focus Area	Concrete Goal
Week 1	Kinematics	Derive \(s + t + u = 0\) and learn planar variables \(X_{i,j}\)
Weeks 2–3	Scalar QFT	Compute the tree-level \(2 \to 2\) amplitude in \(\phi ^{3}\) theory
Week 4	Color & Geometry	Map square & pentagon triangulations to Feynman diagrams

Would you like to jump right into Step 1 and Step 3 together by walking through how the 4-particle square triangulations give the exact physics amplitude \(\frac{1}{s} + \frac{1}{t}\), or would you prefer specific practice problems for relativistic kinematics?
