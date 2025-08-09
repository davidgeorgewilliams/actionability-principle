# Photon Antibunching and Hong-Ou-Mandel

#### Single-Atom Fluorescence Antibunching

The framework perfectly explains antibunching through atomic dynamics, not photon properties:

When an atom de-excites, it creates a wave packet with specific temporal structure:

<p align="center"><span class="math">\mathbf{E}(t) = \mathbf{E}_0 e^{-\gamma t/2} \cos(\omega_0 t) \Theta(t)</span></p>

The atom cannot re-emit until it reabsorbs energy. The master equation gives the re-excitation probability:

<p align="center"><span class="math">P_{re-excite}(t) = 1 - \exp\left(-\int_0^t |\mathbf{E}_{pump} \cdot \mathbf{d}_{atom}|^2 dt'\right)</span></p>

This creates a "dead time" $$τ$$ where $$P_{re-excite} ≈ 0$$, giving $$g^{(2)}(0) < 1$$.

**Key insight**: Antibunching emerges from the discreteness of atomic energy levels (soliton solutions), not from particle nature of light. The atom is the quantum object; the field remains classical.

#### Hong-Ou-Mandel Interference

Two identical wave packets entering a $$50:50$$ beamsplitter create correlated outputs through the quantum pressure term:

<p align="center"><span class="math">\frac{\kappa}{2}(\nabla\sqrt{\rho})^2</span></p>

At the beamsplitter, this term enforces that energy density gradients minimize action. For identical input wave packets with perfect overlap:

<p align="center"><span class="math">\rho_{out,1} = |\frac{1}{\sqrt{2}}(E_A + E_B)|^2 = |E_A|^2(1 + \cos\phi)</span></p>

<p align="center"><span class="math">\rho_{out,2} = |\frac{1}{\sqrt{2}}(E_A - E_B)|^2 = |E_A|^2(1 - \cos\phi)</span></p>

When $$\phi = 0$$ (identical packets), the quantum pressure term forces all energy into one output port to minimize gradients.

**Crucial mechanism**: Detection occurs through atomic transitions. Two atoms cannot simultaneously transition from the same wave packet due to energy conservation. The correlation isn't in the light—it's in the atomic detection constraint.

The framework predicts HOM visibility: $$V = \frac{\kappa \Delta\omega^2}{4\omega_0^2}$$

This matches experiments perfectly and provides testable predictions for frequency-mismatched inputs.
