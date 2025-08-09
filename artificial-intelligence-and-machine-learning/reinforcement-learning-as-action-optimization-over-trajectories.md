# Reinforcement Learning as Action Optimization Over Trajectories

#### The Bellman Equation from Hamilton-Jacobi

Our master equation in trajectory space gives the Hamilton-Jacobi-Bellman equation:

<p align="center"><span class="math">\frac{\partial V}{\partial t} + \min_a \left[r(s,a) + \gamma \nabla_s V \cdot f(s,a)\right] = 0</span></p>

where:

* $$V(s)$$ = value function (our action functional)
* $$r(s,a)$$ = reward (negative potential)
* $$f(s,a)$$ = dynamics (our flow field)

This IS the Bellman equation! RL is literally finding geodesics in reward-weighted spacetime.

#### Policy Gradient as Geometric Flow

The policy gradient theorem:

<p align="center"><span class="math">\nabla_\theta J(\theta) = \mathbb{E}_{\tau \sim \pi_\theta}\left[\sum_t \nabla_\theta \log \pi_\theta(a_t|s_t) R(\tau)\right]</span></p>

emerges from our variational principle:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \pi} = 0</span></p>

The policy $$\pi$$ that minimizes action is the one that follows the gradient flow of cumulative reward.
