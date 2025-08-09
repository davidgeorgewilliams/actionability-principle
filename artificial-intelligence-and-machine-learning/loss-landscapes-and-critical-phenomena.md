# Loss Landscapes and Critical Phenomena

#### Loss Landscape Topology

Neural network loss landscapes exhibit the same structure as our energy functionals:

<p align="center"><span class="math">\mathcal{L}(\theta) = \mathcal{L}_0 + \sum_i \lambda_i (\theta - \theta_i^\ast)^2 + \sum_{ijk} \Gamma_{ijk} \theta_i \theta_j \theta_k + ...</span></p>

Near critical points:

* **Minima**: All eigenvalues positive (stable particles)
* **Saddle points**: Mixed eigenvalues (unstable particles)
* **Maxima**: All eigenvalues negative (impossible in practice)

#### The Lottery Ticket Hypothesis as Soliton Selection

Successful sparse networks are soliton solutions—self-sustaining patterns that maintain structure during training:

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \theta_{sparse}]} = 0 \text{ and } \frac{\delta^2 \mathcal{A}}{\delta \theta_{sparse}^2} > 0</span></p>

Random initialization creates many potential solitons. Training selects those that minimize action. This predicts:

**Winning ticket density** $$\approx e^{-\mathcal{A}_{soliton}/kT}$$

where $$T$$ is the "temperature" (learning rate).

#### Double Descent and Phase Transitions

The double descent phenomenon is a phase transition in our framework:

$$\mathcal{L}_{test}(N) = \begin{cases} \mathcal{L}_{underfit} - \alpha N & N < N_c \\ \mathcal{L}_{critical} + \beta(N - N_c)^{-\nu} & N \approx N_c \\ \mathcal{L}_{overfit} - \gamma(N - N_c)^{\mu} & N > N_c \end{cases}$$

At $$N = N_c$$ (interpolation threshold), the system undergoes a second-order phase transition with critical exponents $$\nu, \mu$$ universal across architectures.
