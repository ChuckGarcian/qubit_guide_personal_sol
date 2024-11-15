# 1.11.6 More time, more memory

## Part A

Consider any transition from one state to another. The total number of possible distinguishable states a state can transition to is $N$. We repeat this for a total of $k$ steps.

Hence, the maximum number of computational paths connecting an input with a specific output is:

$$\Pi^kN = N \times N \ldots \times N = N^k$$

## Part B

The execution time and memory requirement grow with $k$ and $N$.

As shown above, the quantum machine can be configured with $N$ distinguishable states and $N^k$ unique mutually exclusive paths.

In a quantum computational process, each path is associated with a complex amplitude probability $z_i$, $i \in (0, k)$. $z_i$ represents the amplitude contributed by that path.

**Growing $N$:**

- **Time Complexity:** Assuming $k$ is held constant, the time complexity increases polynomially.
- **Space Complexity:** Polynomial for the same reason as time complexity.

**Growing $k$:**

- **Time Complexity:** $\mathcal{O}(N^k)$, exponential in $k$. The number of amplitudes to process is on the order of $\mathcal{O}(N^k)$.
- **Space Complexity:** Exponential in $k$. The number of amplitudes to store is on the order of $\mathcal{O}(N^k)$, which is exponential in $k$.