---
description: From Action Minimization
---

# Universal Function Approximation

#### The Approximation Theorem as Physics

**Theorem**: Any continuous function&#x20;

<p align="center"><span class="math">\mathbb{R}^n \rightarrow \mathbb{R}^m</span> </p>

can be approximated by minimizing our action.

**Proof**: Consider the action functional:

<p align="center"><span class="math">\mathcal{A}[g] = \int ||\nabla g||^2 + \lambda ||g - f||^2 d\mathbf{x}</span></p>

The Euler-Lagrange equation gives:

<p align="center"><span class="math">\nabla^2 g = \lambda(g - f)</span></p>

As $$\lambda \rightarrow \infty$$, $$g\rightarrow f$$ pointwise. A neural network with sufficient capacity implements the Green's function solution:

<p align="center"><span class="math">g(\mathbf{x}) = \sum_i w_i K(\mathbf{x}, \mathbf{x}_i)</span></p>

where $$K$$ is the kernel (implemented by hidden units). This converges to any $$f$$ by the Riesz representation theorem.&#x20;

#### Width vs Depth: The Space-Time Tradeoff

Our framework reveals the fundamental tradeoff:

* **Width** (neurons per layer) = spatial degrees of freedom
* **Depth** (number of layers) = temporal evolution steps

The optimal architecture minimizes total action:

<p align="center"><span class="math">\mathcal{A}_{total} = \mathcal{A}_{spatial} \cdot W + \mathcal{A}_{temporal} \cdot D</span></p>

This predicts:

<p align="center"><span class="math">\frac{W}{D} \approx \sqrt{\frac{\mathcal{A}_{temporal}}{\mathcal{A}_{spatial}}}</span></p>

For vision: $$W/D \approx 100$$ (spatial dominant) For language: $$W/D \approx 10$$ (temporal dominant)
