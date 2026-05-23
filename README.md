# Spectral Amplification by One-Bit Inflow in Collatz Dynamics

**Hiroki Kamanoi**  
Draft — May 2026

Paper C in a series on Collatz dynamics through finite Markov chain theory.

## Overview

This paper introduces a family of Markov kernels $P_{K,m}$ on odd residues modulo $2^K$, parametrized by the number of high bits $m$ averaged over.

The central phenomenon is the **one-bit spectral amplification**:

```
δ_{K,0} = 0  →(1 bit)→  δ_{K,1} ≈ 0.29
```

At $m=0$, the kernel reduces to the deterministic Collatz map with spectral gap zero. At $m=1$, a single bit of high-bit uncertainty jumps the spectral gap to approximately 0.29 — uniformly in $K$.

## Main Results

The paper establishes:

- exact definition of the high-bit averaged kernel $P_{K,m}$;
- Lemma V-stability: the valuation $v_2(3(a+u \cdot 2^K)+1)$ is independent of $u$;
- four computational observations forming a spectral phase diagram;
- the **Open Gap Problem**: $\inf_{K \geq 2} \delta_{K,1} > 0$;
- a systematic negative result: Cheeger inequalities, Weyl perturbation, and Sinkhorn balancing all fail to resolve the open problem;
- identification of the core obstruction: non-normal arithmetic geometry.

## Important Clarification

This repository does **not** claim a proof of the Collatz conjecture.

It also does not claim:

- orbitwise ergodicity or decorrelation;
- a proof of the Open Gap Problem;
- any convergence result for Collatz trajectories.

The heuristic connection to orbitwise decorrelation (Section 6) is explicitly labeled as heuristic. No claims there are asserted as theorems.

## Numerical Component

All spectral observations (positivity, monotonicity, one-bit jump, saturation) are computational results verified for $K = 4, \ldots, 13$. They are not theorems.

## Relation to Other Papers

- Paper A: exact operator structure and renewal systems
- Paper B: exact finite-level mixing geometry, $T_\mathrm{mix}(K) = K-1$
- **Paper C (this paper)**: spectral amplification by one-bit inflow, open gap problem

## Files

- `collatz_spectral_amplification.tex` — LaTeX source
- `collatz_spectral_amplification.pdf` — compiled draft

## Suggested arXiv Categories

Primary: `math.DS`  
Secondary: `math.NT`, `math.PR`, `math.SP`

## License

MIT License


---

## Related work

This repository is part of a series on Collatz dynamics:

| Repository | Description |
|------------|-------------|
| [collatz-renewal-structure](https://github.com/KAMANOI/collatz-renewal-structure) | Paper A: exact renewal structure and operator theory |
| [collatz-finite-mixing-geometry](https://github.com/KAMANOI/collatz-finite-mixing-geometry) | Finite-level mixing geometry |
| [collatz-spectral-amplification](https://github.com/KAMANOI/collatz-spectral-amplification) | Paper C: spectral amplification |
| [collatz-scale-coherence](https://github.com/KAMANOI/collatz-scale-coherence) | Paper D: scale-coherence rigidity |

## Author

Hiroki Kamanoi  
hirokikamanoi@gmail.com  
https://github.com/KAMANOI