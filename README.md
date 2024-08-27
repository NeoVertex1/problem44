# problem44
problem #44 Complexity of the separability problem


$$\text{Definition: A bipartite mixed state } \rho \in \mathcal{D}(\mathbb{C}^d \otimes \mathbb{C}^d) \text{ is separable if and only if:}$$

$$\rho = \sum_{i=1}^k p_i \rho_i^A \otimes \rho_i^B$$

$$\text{where:}$$
<br>

$$- k \text{ is a positive integer}$$

$$- p_i > 0 \text{ and } \sum_{i=1}^k p_i = 1$$

$$- \rho_i^A \in \mathcal{D}(\mathbb{C}^d) \text{ and } \rho_i^B \in \mathcal{D}(\mathbb{C}^d) \text{ are density operators}$$

$$\text{The set of all separable states is denoted as } Sep(d,d).$$

$$\text{Theorem (Caratheodory's theorem for separable states):}$$

$$\text{Any separable state can be written as a convex combination of at most } d^4 \text{ pure product states.}$$

$$\text{Proof sketch:}$$

$$1. \text{The set of separable states is convex.}$$

$$2. \text{The extreme points of this set are pure product states.}$$

$$3. \text{The dimension of the real vector space of Hermitian operators on } \mathbb{C}^d \otimes \mathbb{C}^d \text{ is } d^4.$$

$$4. \text{Apply Caratheodory's theorem for convex sets.}$$

$$\text{Corollary: The set } Sep(d,d) \text{ is closed and convex.}$$

lets visualize the geometry of separable states:

![Geometry Of Separable States](https://github.com/NeoVertex1/problem44/blob/main/Geometry_Separable_States.svg)



$$\text{Problem: ε-weak membership for } Sep(d,d)$$

$$\text{Input:}$$

$$- \text{A density matrix } \rho \in \mathcal{D}(\mathbb{C}^d \otimes \mathbb{C}^d)$$

$$- \text{A parameter } \epsilon > 0$$

$$\text{Promise:}$$

$$\text{Either } \rho \in Sep(d,d) \text{ or } \rho \text{ is ε-far from any state in } Sep(d,d) \text{ in trace distance.}$$

$$\text{Output:}$$

$$\text{"YES" if } \rho \in Sep(d,d), \text{ "NO" if } \rho \text{ is ε-far from } Sep(d,d).$$

$$\text{Trace Distance:} D(\rho, \sigma) = \frac{1}{2} \|\rho - \sigma\|_1 = \frac{1}{2} \text{Tr}\sqrt{(\rho - \sigma)^\dagger(\rho - \sigma)}$$

$$\text{ε-far condition:} \min_{\sigma \in Sep(d,d)} D(\rho, \sigma) > \epsilon$$

$$\text{Theorem (Gurvits, 2003):}$$

$$\text{The ε-weak membership problem for } Sep(d,d) \text{ is NP-hard for } \epsilon \leq 1/\text{poly}(d).$$

$$\text{Open Question:}$$

$$\text{Is there a quasi-polynomial time algorithm for constant } \epsilon > 0 \text{?}$$


![ε-weak membership visualization](https://github.com/NeoVertex1/problem44/blob/main/%CE%B5-weak_membership_visualization.svg)


