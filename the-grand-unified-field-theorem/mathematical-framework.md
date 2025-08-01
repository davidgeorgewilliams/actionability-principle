# Mathematical Framework

### Scale-Dependent Parameters

The theory includes scale-dependent couplings that flow according to renormalization group equations:

<p align="center"><span class="math">\frac{d\kappa}{d\log k} = \beta_\kappa(\kappa, V, \mathcal{R})</span> <br><br><span class="math">\frac{dV}{d\log k} = \beta_V(\kappa, V, \mathcal{R})</span><br><br><span class="math">\frac{d\mathcal{R}}{d\log k} = \beta_\mathcal{R}(\kappa, V, \mathcal{R})</span></p>

where $$k$$ is the energy scale.

### Dimensional Analysis

In natural units where $$\hbar = c = k_B = 1$$:

* $$[\rho]$$: $$Energy^4$$ (energy **density** - energy per volume)
* $$[\mathbf{j}]$$: $$Energy^4$$ (energy **flux** - energy flow per area per time)
* $$[\kappa]$$: $$Energy^{-2}$$ (quantum scale)
* $$[V]$$: $$Energy^4$$ (potential scale)
* $$[\mathcal{R}]$$: $$Energy^4$$ (curvature scale)

### Computational Methods

* **Perturbative**: Expand around equilibrium solutions&#x20;
* **Non-perturbative**: Numerical integration of master equations
* **Effective field theory**: Integrate out high-energy modes&#x20;
* **Monte Carlo**: Statistical sampling of field configurations

### **What Are Natural Units?**

In everyday physics, we use different units:

* **Length**: meters (m)
* **Time**: seconds (s)
* **Mass**: kilograms (kg)
* **Energy**: joules (J)

**Natural units** set the fundamental constants equal to 1:

* $$ℏ = 1$$ (quantum mechanics scale)
* $$c = 1$$ (relativity scale)
* $$k_B = 1$$ (thermodynamics scale)

### **Why This Simplifies Everything**

When $$ℏ = c = k_B = 1$$, we can measure **everything** in terms of **energy**:

#### **From the Constants**:

* $$ℏ$$ has dimensions $$[Energy][Time] = 1 → [Energy] = [Time]⁻¹$$
* $$c$$ has dimensions $$[Length][Time]⁻¹ = 1 → [Length] = [Time]$$
* Therefore: $$[Energy] = [Time]⁻¹ = [Length]⁻¹$$

**Everything is measured in energy units!**

### **Working Out Each Dimension**

#### **1. Energy Density ρ**

#### **Regular units**: $$[Energy]/[Volume] = [Energy]/[Length]³$$

**Natural units**:

* $$[Length]³ = [Energy]⁻³ (since [Length] = [Energy]⁻¹)$$
* So $$[ρ] = [Energy]/[Energy]⁻³ = Energy⁴$$

#### **2. Energy Current j**

**Regular units**: $$[Energy]/[Area]/[Time] = [Energy]/[Length]²/[Time]$$

**Natural units**:

* $$[Length]² = [Energy]⁻²$$
* $$[Time] = [Energy]⁻¹$$
* So $$[j] = [Energy]/[Energy]⁻²/[Energy]⁻¹ = [Energy] × [Energy]² × [Energy] = Energy⁴$$

#### **3. Quantum Parameter κ**

From our action, $$κ$$ appears in: $$\frac{\kappa}{2}(\nabla \sqrt{\rho})²$$&#x20;

**Dimensional check**:

* $$\sqrt{\rho}$$ has dimensions $$[Energy]^2$$
* $$\nabla\sqrt{\rho}$$ has dimensions $$[Energy]^2/[Length] = [Energy]^2 \times [Energy] = [Energy]^3$$
* $$(\nabla\sqrt{\rho})^2$$ has dimensions $$[Energy]^6$$

For the term to have Energy⁴ (to match the action):

* $$[\kappa] \times [\text{Energy}]^6 = [\text{Energy}]^4$$
* Therefore $$[\kappa] = \textbf{Energy}^{-2}$$

#### **4. Potential V and Curvature R**

Both potential $$V$$ and curvature $$\mathcal{R}$$ appear directly in the action and must contribute $$Energy⁴$$ to match the overall action dimensions.

### **Physical Intuition**

**Why Energy⁴?**

* Our action integrates over **4D spacetime** (3 space + 1 time)
* Each integration contributes $$[Length] = [Energy]⁻¹$$
* So the integrand must have dimensions $$[Energy]⁴$$ to make the action dimensionless

### **The Beauty of Natural Units**

Instead of tracking meters, seconds, kilograms separately, **everything is just powers of energy**:

* **Big energy**: Short distance, high frequency, heavy mass
* **Small energy**: Long distance, low frequency, light mass

**Example**: In natural units, the proton mass $$≈ 1 GeV$$ is the same number as its rest energy!
