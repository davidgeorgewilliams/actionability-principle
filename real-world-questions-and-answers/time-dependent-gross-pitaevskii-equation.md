# Time-Dependent Gross-Pitaevskii Equation

**From StackExchange Physics:** _"Why can we replace field operators by their expectation? Can we derive GPE from many-body Schrödinger equation? What's the logic of the action principle? Why do all approaches give the same GPE?"_

### Answer: The Master Equation Unifies All GPE Derivations

#### The Fundamental Truth

The Gross-Pitaevskii equation emerges from our master equation when energy density forms a coherent condensate:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \rho} = -\Gamma[\rho] \frac{\partial \rho}{\partial T}</span></p>

For Bose-Einstein condensates, $$ρ$$ becomes macroscopically occupied in a single quantum state.

#### 1. Why Replace Operators with Expectations?

When $$N₀ >> 1$$ particles occupy the same state, quantum fluctuations become negligible:

<p align="center"><span class="math">\hat{\Psi} = \sqrt{N_0}\psi_0 + \delta\hat{\Psi}</span></p>

The relative fluctuation:&#x20;

<p align="center"><span class="math">\frac{\langle(\delta\hat{\Psi})^2\rangle}{N_0} \sim \frac{1}{\sqrt{N_0}} \to 0</span></p>

This is valid because our framework shows condensates are stable solitons where $$ρ = |ψ|²$$ becomes classical-like. The operator replacement works when:

* $$N₀ >> 1$$ (macroscopic occupation)
* Interactions are weak (preserves coherence)
* Temperature $$T << T_c$$ (thermal fluctuations suppressed)

#### 2. From Many-Body Schrödinger to GPE

Starting with $$N$$-body wavefunction $$Ψ(r₁,...,rₙ,t)$$ and the product ansatz:&#x20;

<p align="center"><span class="math">\Psi = \prod_{i=1}^N \chi_0(\mathbf{r}_i,t)</span></p>

Substituting into the many-body Schrödinger equation and using our framework's variational principle:

<p align="center"><span class="math">\langle\Psi|\hat{H}|\Psi\rangle = N\int|\nabla\chi_0|^2 + \frac{N(N-1)}{2}\int|\chi_0|^4 V_{int}</span></p>

Taking variation with respect to $$χ₀\ast$$ gives GPE:&#x20;

<p align="center"><span class="math">i\hbar\frac{\partial\chi_0}{\partial t} = -\frac{\hbar^2}{2m}\nabla^2\chi_0 + V_{ext}\chi_0 + gN|\chi_0|^2\chi_0</span></p>

The product state works because interactions create an effective mean field that maintains coherence.

#### 3. Action Principle Logic

The action approach directly implements our master equation. The Lagrangian:&#x20;

<p align="center"><span class="math">L = \int\left[i\hbar\psi^\ast\dot{\psi} - \mathcal{H}[\psi]\right]d^3r</span></p>

is exactly our action functional with:

* Kinetic term: $$\frac{|\mathbf{j}|^2}{2\rho} → \frac{\hbar^2}{2m}|\nabla\psi|^2$$
* Interaction: $$V(\rho) →\frac{g}{2}|\psi|^4$$&#x20;
* Quantum pressure: Built into the gradient term

The variation $$δ∫L dt = 0$$ is precisely our condition $$\frac{\delta\mathcal{A}}{\delta\rho} = 0$$.

#### 4. Why All Approaches Converge

All three methods are different projections of the same underlying physics:

**Master Equation** → **GPE** via:

* Field operators: Statistical limit of quantum fields
* Product ansatz: Mean-field approximation
* Action principle: Direct variational formulation

They must agree because they're solving the same problem: finding the configuration that minimizes action for a macroscopic condensate.

#### The Deep Connection

The GPE is the Schrödinger equation for the condensate wavefunction $$ψ = √ρ e^(iS/ℏ)$$:

\$$i\hbar\frac{\partial\psi}{\partial t} = -\frac{\hbar^2}{2m}\nabla^2\psi + V\_{ext}\psi + g|\psi|^2\psi\$$

This emerges from our master equation when:

* Dissipation $$Γ[ρ] → 0$$ (coherent state)
* Quantum pressure dominates (maintains condensate)
* $$N₀ >> 1$$ (classical-like amplitude)

The nonlinear term $$g|ψ|²ψ$$ comes from the self-interaction of the condensate with its own density field—the universe computing the optimal configuration for macroscopic quantum coherence.
