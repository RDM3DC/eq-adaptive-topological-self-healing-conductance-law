# Adaptive Topological Self-Healing Conductance Law


<!-- HERO_ANIMATION:BEGIN -->
![Adaptive topological self-healing conductance law](images/topological_self_healing.gif)

_Hero animation: **Adaptive topological self-healing conductance law**. [Download high-resolution MP4](images/topological_self_healing.mp4)._
<!-- HERO_ANIMATION:END -->

**ID:** `eq-adaptive-topological-self-healing-conductance-law`  
**Tier:** derived  
**Score:** 85  
**Units:** OK  
**Theory:** PASS-WITH-ASSUMPTIONS  

## Equation

$$
\frac{d g_e}{dt} = \alpha_G(S)\,|J_e|\,e^{i\theta_{R,e}} - \mu_G(S)\,g_e - \lambda_s\,g_e\,\sin^2\!\left(\frac{\theta_{R,e}}{2\pi_a}\right)
$$

## Description

Adaptive complex edge-conductance law for a damaged topological lattice with history-resolved phase memory. Each edge coupling g_e is reinforced by local bond activity |J_e| in the lifted phase direction e^{i theta_{R,e}}, decays at an entropy-gated rate mu_G(S), and is selectively suppressed when the resolved phase becomes incompatible with the current adaptive ruler pi_a. In a QWZ-style two-band block lattice, the same scalar update multiplies fixed 2x2 bond operators, so the law acts as a local self-healing rule for restoring boundary-dominated transport after bond damage.

## Assumptions

- g_e is a complex edge conductance or adaptive scalar bond multiplier with units of conductance; J_e is the corresponding complex bond current/activity, so alpha_G has units 1/(V*s), mu_G and lambda_s have units 1/s, and theta_{R,e}, pi_a are dimensionless.
- theta_{R,e} is updated by a history-resolved clipped phase-lift rule relative to the previous edge phase, so branch continuity is retained and principal-branch aliasing is avoided over bounded increments.
- S is a nonnegative entropy-like state that gates reinforcement and decay through alpha_G(S) and mu_G(S); pi_a may be constant or adapt by a companion ruler ODE.
- The QWZ interpretation assumes each adaptive scalar g_e multiplies a fixed nearest-neighbour 2x2 bond block, while onsite mass m sets the bulk topological regime.
- The suppression factor sin^2(theta_{R,e}/(2*pi_a)) is a bounded frustration penalty rather than a universal microscopic dissipation law.

## Repository Structure

```
images/       # Visualizations, plots, diagrams
derivations/  # Step-by-step derivations and proofs
simulations/  # Computational models and code
data/         # Numerical data, experimental results
notes/        # Research notes and references
```

## Links

- [TopEquations Registry](https://rdm3dc.github.io/TopEquations/registry.html)
- [TopEquations Main Repo](https://github.com/RDM3DC/TopEquations)
- [Certificates](https://rdm3dc.github.io/TopEquations/certificates.html)

---
*Part of the [TopEquations](https://github.com/RDM3DC/TopEquations) project.*
