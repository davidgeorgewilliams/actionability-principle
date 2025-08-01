# The Energy-Information Master Equation

### The Unified Action

The complete action that generates all of physics is:

<p align="center"><span class="math">S[\rho, \mathbf{j}] = \int d^D X \, dT \, \sqrt{|\det G_{AB}|} \left[ \frac{|\mathbf{j}|^2}{2\rho} + V(\rho) + \frac{\kappa}{2}(\nabla \sqrt{\rho})^2 + \mathcal{R}[\rho] \right]</span>​</p>

where:

* $$G_{AB}(\mathbf{X})$$: Emergent metric tensor on master space
* $$\frac{|\mathbf{j}|^2}{2\rho}$$​: Kinetic energy of probability flow
* $$V(\rho)$$: Potential energy landscape
* $$\frac{\kappa}{2}(\nabla \sqrt{\rho})^2$$: Quantum pressure term (with $$\kappa \sim \hbar^2$$, and $$h$$ is the reduced Planck's constant $$1.055 \times 10^{-34} \text{J}\cdot\text{s}$$)
* $$\mathcal{R}[\rho]$$ Information geometry curvature

#### The Master Equations

Taking functional derivatives yields the coupled evolution equations:

<p align="center"><span class="math">\frac{\delta S}{\delta \rho} = -\Gamma[\rho] \frac{\partial \rho}{\partial T}</span><br><br><span class="math">\frac{\delta S}{\delta \mathbf{j}} = -\Lambda[\mathbf{j}] \frac{\partial \mathbf{j}}{\partial T}</span></p>

### Explicit Forms

**Continuity equation**:

<p align="center"><span class="math">\frac{\partial \rho}{\partial T} + \nabla \cdot \mathbf{j} = \Gamma[\rho]</span></p>

**Flow equation**:

<p align="center"><span class="math">\frac{\partial \mathbf{j}}{\partial T} + \nabla \left(\frac{|\mathbf{j}|^2}{2\rho} + V + \frac{\kappa}{2\sqrt{\rho}}\nabla^2\sqrt{\rho} + \frac{\delta \mathcal{R}}{\delta \rho}\right) = \Lambda[\mathbf{j}]</span></p>
