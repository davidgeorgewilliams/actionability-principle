# Deep Neural Networks as Discretized Flow Fields

#### The Flow Interpretation

A neural network with LL L layers implements discretized flow in information space:

<p align="center"><span class="math">\mathbf{x}_{l+1} = f_l(\mathbf{x}_l; \theta_l)</span></p>

This is precisely the discrete evolution of our current field:

<p align="center"><span class="math">\mathbf{x}(t + \Delta t) = \mathbf{x}(t) + \Delta t \cdot \mathbf{j}(\mathbf{x}(t), t)</span></p>

Each layer represents a time step $$\Delta t$$ in master time $$T$$. The parameters $$\theta$$ determine the flow field at each point.

#### Deriving Backpropagation from Action Minimization

The loss function is our action functional:

<p align="center"><span class="math">\mathcal{L}(\theta) = \int p(\mathbf{x}) \left[\frac{1}{2}||y - f_\theta(\mathbf{x})||^2\right] d\mathbf{x}</span></p>

Taking the functional derivative:

<p align="center"><span class="math">\frac{\delta \mathcal{L}}{\delta f_l} = \frac{\partial \mathcal{L}}{\partial f_l} + \sum_{k>l} \frac{\partial \mathcal{L}}{\partial f_k} \frac{\partial f_k}{\partial f_l}</span></p>

This IS the backpropagation equation! The chain rule emerges naturally from the action principle applied to compositional flows.

#### Depth as Computational Time

Our framework reveals why depth matters:

<p align="center"><span class="math">\mathcal{A}[f_\theta] = \int_0^L \left[\frac{||\partial_l f||^2}{2} + V(f_l) + \frac{\kappa}{2}||\nabla f_l||^2\right] dl</span></p>

Deeper networks allow more "time" for the information flow to develop complex transformations. The optimal depth $$L^\ast$$  minimizes total action:

<p align="center"><span class="math">L^\ast = \sqrt{\frac{2\mathcal{C}(f_{target})}{\kappa}}</span>​​</p>

where $$\mathcal{C}(f_{target})$$ measures target function complexity.
