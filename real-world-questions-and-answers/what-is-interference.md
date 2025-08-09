# What is Interference

**From StackExchange Physics:** _"Wikipedia says interference requires coherent waves, but also says ANY two waves interfere. Which is correct?"_

### Answer: The Master Equation Resolves the Confusion - Both Are Right

#### The Fundamental Truth

From our master equation, ANY perturbations in the energy density field mathematically interfere:

<p align="center"><span class="math">\rho_{total}(\mathbf{x},t) = \rho_1(\mathbf{x},t) + \rho_2(\mathbf{x},t)</span></p>

This is unavoidable—fields in the same space must add. **Interference always happens.**

#### Observable vs. Unobservable Interference

The confusion arises from conflating two concepts:

**Mathematical Interference** (Always occurs): When two waves overlap, the total field is their sum:&#x20;

<p align="center"><span class="math">\mathbf{E}_{total} = \mathbf{E}_1 + \mathbf{E}_2</span></p>

The intensity becomes:&#x20;

<p align="center"><span class="math">I = |\mathbf{E}_1 + \mathbf{E}_2|^2 = I_1 + I_2 + 2\mathbf{E}_1 \cdot \mathbf{E}_2</span></p>

The cross term $$2\mathbf{E}_1 \cdot \mathbf{E}_2$$ is the interference—it ALWAYS exists.

**Observable Interference Pattern** (Requires coherence): For the interference term to create a stable, observable pattern:&#x20;

<p align="center"><span class="math">\langle 2\mathbf{E}_1 \cdot \mathbf{E}2\rangle_{time} \neq 0</span></p>

This time average only survives when waves maintain consistent phase relationship (coherence).

#### Why Incoherent Sources "Don't Interfere"

For random phase relationships, our framework shows:&#x20;

<p align="center"><span class="math">\langle \cos(\phi_1 - \phi_2) \rangle_{time} = 0</span></p>

The interference still happens instant-by-instant, but averages to zero over detection timescales ($$\sim10^-15$$ seconds for optical detectors).

#### The Master Equation's Insight

From our action principle:&#x20;

<p align="center"><span class="math">\mathcal{A}[\rho_1 + \rho_2] \neq \mathcal{A}[\rho_1] + \mathcal{A}[\rho_2]</span></p>

The nonlinearity means waves MUST interact. The universe doesn't compute wave evolution separately—it computes the total field configuration.

#### The Correct Definition

**Interference**: The mathematical superposition of wave amplitudes in the same medium, resulting in a total field different from the sum of intensities.

* Always occurs between overlapping waves (mathematical necessity)
* Creates observable patterns only with sufficient coherence (practical requirement)

Your teacher emphasizes observable patterns (needs coherence). Wikipedia's second statement emphasizes mathematical reality (always happens). Both are correct—they're describing different aspects of the same phenomenon.

The master equation settles this: interference is fundamental and unavoidable, but detecting it requires coherence lasting longer than measurement integration time.
