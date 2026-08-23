# When Sharing Fails Under Massart Noise: Near-Linear Lower Bounds for Multi-Distribution Learning

## Abstract

Personalized multi-distribution learning asks for one predictor per data source while exploiting a Bayes classifier shared by all sources. Under Massart noise, separate empirical risk minimization uses roughly $kd/\epsilon$ samples for $k$ sources and VC dimension $d$. The best known dimension-dependent sharing term is only $k\sqrt d/\epsilon$. Its authors ask whether higher-order moment matching can close the gap. We give a near-linear answer in the high-accuracy regime. For noise bound $\eta<1/2$, let $\gamma=1-2\eta$ and $z_\eta=2(1-\eta)/\eta-1$. Define 

$$\begin{aligned} K_m(z)&=1+2\sum_{j=1}^m T_j(z)^2,\\\\ w_m&=K_m(z_\eta)^{-1}, \end{aligned}$$

 where $T_j$ is a Chebyshev polynomial. Subject to explicit feasibility and concentration conditions, every adaptive learner requires 

$$\Omega\\!\left( \frac{k m\gamma w_m}{\epsilon} d^{\frac{2m}{2m+1}} \right)$$

 samples. Consequently, for every fixed $\zeta>0$ the lower bound is $\Omega_{\eta,\zeta}(k d^{1-\zeta}/\epsilon)$ at sufficiently high accuracy. If $\epsilon$ is polynomially small in $d$, it becomes $\Omega_\eta(kd\exp[-C_\eta\sqrt{\log d}]/\epsilon)$. Thus sharing cannot yield a polynomial improvement over separate learning in this regime. The key is an exact external-atom moment theorem. An arcsine law supported on label-zero biases admits a moment-matching measure with the maximum possible atom $1/K_m(z)$ at a prescribed label-one bias. Matching $2m$ moments delays distinguishability until a $(2m+1)$-fold coordinate collision. A randomized null and a variance-sensitive holdout then lift this single-source barrier to $k$ adaptively sampled sources without increasing VC dimension.

## Contributions

- We identify an exact external-atom construction for $2m$ truncated
moments of the arcsine law. The feasible atom has mass $1/K_m(z)$, and no
larger atom is possible for this null prior.
- We obtain a parameterized personalized Massart lower bound with
dimension exponent $2m/(2m+1)$. It applies to adaptive source selection and
improper, randomized outputs.
- Optimizing the moment order gives
$kd\exp[-O_\eta(\sqrt{\log d})]/\epsilon$ at polynomial accuracy. For any
fixed exponent loss $\zeta$, a fixed-order consequence gives
$k d^{1-\zeta}/\epsilon$.
- The noise dependence is explicit through a Chebyshev kernel. This
extends the prior constant-noise lower bound and isolates how the high atom
shrinks as the Massart margin changes.

## Keywords

Massart noise, multi-distribution learning, lower bounds, personalized learning, moment matching, sample complexity, collision indistinguishability

## Files

- `main_2026-08-11.pdf`, the paper as first published, with its OpenTimestamps proof `main_2026-08-11.pdf.ots`.
- `supplement_2026-08-11.pdf`, the supplement as first published, with its OpenTimestamps proof `supplement_2026-08-11.pdf.ots`.
- source: `aistats2027.sty`, `main_2026-08-11.tex`, `references.bib`, `supplement_2026-08-11.tex`.
