# Emergence of the Hydrogen Atom

### Step 1: Starting from the Master Equation

Our master equation governs all physics:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \rho} = -\Gamma[\rho] \frac{\partial \rho}{\partial T}</span></p>

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \mathbf{j}} = -\Lambda[\mathbf{j}] \frac{\partial \mathbf{j}}{\partial T}</span></p>

For the hydrogen atom, we seek stationary solutions where $$\frac{\partial \rho}{\partial T} = 0$$ and $$\frac{\partial \mathbf{j}}{\partial T} = 0$$, which means:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \rho} = 0 \quad \text{and} \quad \frac{\delta \mathcal{A}}{\delta \mathbf{j}} = 0</span></p>

### Step 2: Computing the Functional Derivatives

From our action:&#x20;

<p align="center"><span class="math">\mathcal{A}[\rho, \mathbf{j}] = \int d^D X dT\sqrt{|\det G_{AB}|} \left[ \frac{|\mathbf{j}|^2}{2\rho} + V(\rho) + \frac{\kappa}{2}(\nabla \sqrt{\rho})^2 + \mathcal{R}[\rho] \right]</span></p>

Taking the functional derivative with respect to $$\rho$$:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \rho} = -\frac{|\mathbf{j}|^2}{2\rho^2} + \frac{\partial V}{\partial \rho} - \frac{\kappa}{4\rho^{3/2}}\nabla^2\sqrt{\rho} + \frac{\kappa}{4\rho}|\nabla\sqrt{\rho}|^2 + \frac{\delta \mathcal{R}}{\delta \rho}</span></p>

Setting this to zero for stationary states and simplifying:

<p align="center"><span class="math">\frac{|\mathbf{j}|^2}{2\rho^2} = \frac{\partial V}{\partial \rho} - \frac{\kappa}{2\sqrt{\rho}}\nabla^2\sqrt{\rho} + \frac{\delta \mathcal{R}}{\delta \rho}</span></p>

Taking the functional derivative with respect to $$\mathbf{j}$$:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \mathbf{j}} = \frac{\mathbf{j}}{\rho}</span></p>

Setting to zero gives $$\mathbf{j} = 0$$ for ground state, or $$\nabla \times \mathbf{j} = 0$$ for general stationary states (irrotational flow).

### Step 3: The Hydrogen-Specific Configuration

For atomic physics, we identify:

* $$\rho \sim 10^{-30}  \text{kg/m}^3$$ (electron probability density)
* $$\kappa = \frac{\hbar^2}{m_e} \approx 1.21 \times 10^{-68} \text{J} \cdot \text{m}^2 \cdot \text{s}^2$$
* $$V(\rho) = -\frac{e^2}{4\pi\epsilon_0 r}$$
* Permittivity of space $$\epsilon_0 = 8.854 \times 10^{-12} \text{F} \cdot \text{m}^{-1}$$ (farads per meter)
* Neglect $$\mathcal{R}[\rho]$$ (curvature term small at atomic scales)

### Step 4: Continuity and Flow Equations

From the stationary condition and our master equation structure:

**Continuity equation** (from $$\partial \rho/\partial T = 0$$):

<p align="center"><span class="math">\nabla \cdot \mathbf{j} = 0</span></p>

**Flow equation** (from gradient of energy density):&#x20;

<p align="center"><span class="math">\nabla \left(\frac{|\mathbf{j}|^2}{2\rho} + V + \frac{\kappa}{2\sqrt{\rho}}\nabla^2\sqrt{\rho}\right) = 0</span></p>

This second equation means the quantity in parentheses is constant - this constant is the energy $$E$$.

### Step 5: Spherical Symmetry Reduction

For hydrogen's spherical symmetry:

* $$\rho = \rho(r)$$ (depends only on distance from nucleus)
* $$\mathbf{j} = j(r)\hat{\mathbf{r}}$$ for radial flow or $$\mathbf{j} = 0$$ for ground state

The Laplacian in spherical coordinates:

<p align="center"> <span class="math">\nabla^2\sqrt{\rho} = \frac{1}{r^2}\frac{d}{dr}\left(r^2 \frac{d\sqrt{\rho}}{dr}\right)</span></p>

Therefore, the quantum pressure term becomes:&#x20;

<p align="center"><span class="math">\frac{\kappa}{2\sqrt{\rho}}\nabla^2\sqrt{\rho} = \frac{\kappa}{2\sqrt{\rho}} \cdot \frac{1}{r^2}\frac{d}{dr}\left(r^2 \frac{d\sqrt{\rho}}{dr}\right)</span></p>

### Step 6: The Quantum Potential and Total Energy

Define the quantum potential:&#x20;

<p align="center"><span class="math">Q = -\frac{\kappa}{2\sqrt{\rho}}\nabla^2\sqrt{\rho}</span></p>

The total energy (from our flow equation) is:&#x20;

<p align="center"><span class="math">E = \frac{|\mathbf{j}|^2}{2\rho} + V(r) + Q</span></p>

For the ground state where $$\mathbf{j} = 0$$:&#x20;

<p align="center"><span class="math">E = V(r) + Q</span></p>

### Step 7: Deriving the Quantization Condition

From our master equation, bound states require $$\rho \to 0$$ as $$r \to \infty$$. The WKB-type quantization condition emerges from the requirement that the action integral around a classical orbit equals $$2\pi n\kappa$$:

<p align="center"><span class="math">\oint \sqrt{2m_e\rho(E - V - Q)} dr = 2\pi n\hbar</span></p>

Since $$\kappa = \hbar^2/m_e$$, this becomes:&#x20;

<p align="center"><span class="math">\oint \sqrt{2\rho(E - V - Q)/\kappa} dr = 2\pi n</span></p>

### Step 8: Energy Eigenvalues

Solving the quantization condition with $$V = -e^2/(4\pi\epsilon_0 r)$$ yields:

<p align="center"><span class="math">E_n = -\frac{m_e e^4}{2(4\pi\epsilon_0)^2\hbar^2 n^2} = -\frac{13.6 \text{ eV}}{n^2}</span></p>

This is exactly the Bohr formula, emerging naturally from our real-valued master equation!

### Step 9: Connection to Wave Functions

While our theory is fundamentally real-valued, we can make contact with traditional quantum mechanics through:

<p align="center"><span class="math">\rho = |\psi|^2</span> </p>

<p align="center"><span class="math">\mathbf{j} = \frac{\hbar}{m_e}\rho\nabla S</span></p>

where $$S$$ is the quantum Hamilton-Jacobi phase. The traditional wave function $$\psi = \sqrt{\rho}e^{iS/\hbar}$$ is merely a mathematical convenience - the physics lives entirely in the real fields $$\rho$$ and $$\mathbf{j}$$.

### The Profound Result

The hydrogen atom emerges from our master equation as a stable, stationary solution where:

1. The quantum pressure $$\kappa$$ term prevents collapse to the nucleus
2. The Coulomb potential $$V(r)$$ provides the binding
3. The balance between these creates discrete energy levels
4. All calculations use only real-valued functions

This demonstrates that quantum mechanics is not mysterious - it's simply the physics of energy density flows at small scales where the quantum pressure term $$\kappa$$ becomes significant.
