# problem44
problem #44 Complexity of the separability problem


$$\text{Definition: A bipartite mixed state } \rho \in \mathcal{D}(\mathbb{C}^d \otimes \mathbb{C}^d) \text{ is separable if and only if:}$$

\rho = \sum_{i=1}^k p_i \rho_i^A \otimes \rho_i^B

\text{where:}
- k \text{ is a positive integer}
- p_i > 0 \text{ and } \sum_{i=1}^k p_i = 1
- \rho_i^A \in \mathcal{D}(\mathbb{C}^d) \text{ and } \rho_i^B \in \mathcal{D}(\mathbb{C}^d) \text{ are density operators}

\text{The set of all separable states is denoted as } Sep(d,d).

\text{Theorem (Caratheodory's theorem for separable states):}
\text{Any separable state can be written as a convex combination of at most } d^4 \text{ pure product states.}

\text{Proof sketch:}
1. \text{The set of separable states is convex.}
2. \text{The extreme points of this set are pure product states.}
3. \text{The dimension of the real vector space of Hermitian operators on } \mathbb{C}^d \otimes \mathbb{C}^d \text{ is } d^4.
4. \text{Apply Caratheodory's theorem for convex sets.}

\text{Corollary: The set } Sep(d,d) \text{ is closed and convex.}
