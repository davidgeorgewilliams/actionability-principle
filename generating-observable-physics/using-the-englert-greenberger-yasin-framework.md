---
description: Visibility vs. Distinguishability in Recoiling-Slit Interferometry
---

# Using the Englert-Greenberger-Yasin Framework

#### The Mathematical Precision That Destroys Vague Claims

The physics community has long conflated two distinct concepts: visibility loss and which-way information. The rigorous **Englert-Greenberger-Yasin (EGY) duality relation** provides operational, measurable quantities that cut through this confusion and expose exactly where papers like the MIT team's mislead through imprecise language.

#### The EGY Duality Relation

The fundamental bound is: $$V^2 + D^2 \leq 1$$

Where:

* **V** = fringe visibility = $$(I_{max} - I_{min})/(I_{max} + I_{min})$$
* **D** = path distinguishability = maximum path-guessing advantage from the which-way marker

This isn't philosophy—it's mathematics. And it reveals something crucial: $$V$$ **can drop without** $$D$$ **increasing**.

### The MIT Paper's Hidden Confession

Lin et al. make an extraordinary admission that undermines the standard narrative. They explicitly state:

> "the apparent loss of fringe contrast is **not related to which-way information**"

They're acknowledging that visibility loss doesn't necessarily mean path information! This isn't buried in a footnote—it's their own conclusion for Configuration C with long pulses.

Let's use their own analysis within the EGY framework to expose the truth.

### Configuration C: Where the Truth Emerges

#### Short Pulses

The atom-photon system becomes entangled:

* Atom in $$|0$$⟩: symmetric interference pattern
* Atom in $$|1⟩$$: π-shifted interference pattern
* Unconditional visibility: $$V = 1 - 2|β|²$$

But what's the distinguishability $$D$$? For small $$β$$:

* Probability atom stays in $$|0⟩: ≈ 1 - |β|²$$
* Probability atom goes to $$|1⟩: ≈ |β|²$$
* Optimal path discrimination: $$D ≈ O(|β|)$$

The crucial insight: $$V$$ **drops as** $$|β|²$$ **while** $$D$$ **only rises as** $$|β|$$. The visibility loss dramatically exceeds the actual which-way information!

#### Long Pulses: The Complete Vindication

With long pulses, the MIT team finds:

* Two frequency components appear (unshifted and shifted by $$ω_{trap}$$)
* Each frequency shows **full contrast** interference
* Only when frequencies are mixed does $$V$$ appear reduced

Their solution: Add a dispersive element that phase-shifts one frequency by π, and **full visibility returns at a single detector**.

In EGY terms: $$V$$ **dropped due to spectral mixing, but** $$D$$ **remained near zero** because no actual path information was recorded.

### The 2D Extension

When the MIT team adds longitudinal motion (Configuration $$D$$), something remarkable happens:

* Longitudinal displacement |α⟩ can be **detected with \~100% probability**
* Yet it **doesn't affect interference at all**

Why? Because longitudinal motion is **common-mode**—both paths create the same displacement. In the EGY framework:

* Detection probability ≈ 100%
* Path distinguishability $$D = 0$$
* Visibility $$V$$ = unchanged

This destroys the naive interpretation that "detection = which-way information."

### The Quantum Eraser: Not Magic, Just Math

What's really happening in quantum eraser experiments:

1. The "eraser" is a **unitary rotation** on the which-way register
2. It maps path-correlated states onto interference-basis states
3. Post-selection reveals complementary high-$$V$$ fringes

In the EGY framework:

* Before erasure: Low $$V$$, some $$D$$
* After erasure + post-selection: High $$V$$, zero $$D$$ (for each post-selected subset)

It's not "erasing information"—it's rotating the measurement basis.

### What We Should Demand from Experimentalists

Using the EGY framework, all interferometry papers should report:

1. **Both** $$V$$ **and** $$D$$ as functions of all parameters
2. **Verification of** $$V² + D² ≤ 1$$ with error bars
3. **Conditional** $$V$$ after frequency/state discrimination
4. **Common vs. differential mode analysis** for all degrees of freedom

The MIT paper only reports $$V$$, not $$D$$—a critical omission that enables loose language about "which-way information."

### The Precise Critique

The MIT paper demonstrates regimes where fringe visibility $$V$$ drops substantially while path distinguishability $$D$$ remains low, violating the common claim that "visibility loss implies which-way information." In Configuration C with long pulses, they explicitly acknowledge that visibility reduction is "not related to which-way information" but rather to spectral mixing that can be undone with frequency discrimination. Their 2D extension shows that common-mode recoil can be detected with near-certainty while leaving $$V$$ unchanged—proving that detectability ≠ distinguishability.

All such experiments should report both $$V$$ and $$D$$, verify $$V² + D² ≤ 1$$, and carefully distinguish between:

* **Entanglement-induced mixing** (reduces $$V$$, doesn't necessarily increase $$D$$)
* **Actual path distinguishability** (increases $$D$$, must reduce $$V$$)

The term "which-way information" should be reserved for cases where $$D$$ demonstrably increases, not wherever $$V$$ decreases.

### The Master Equation Connection

Our framework naturally incorporates this distinction:

* **Continuous waves** create interference (determining $$V$$)
* **Discrete atomic states** can become entangled with the field
* **Entanglement** reduces unconditional V without necessarily creating distinguishable path markers
* **Common-mode** effects don't break interference because they don't correlate with paths

The master equation:&#x20;

<p align="center"><span class="math">\frac{\delta \mathcal{A}}{\delta \rho} = -\Gamma[\rho] \frac{\partial \rho}{\partial T}</span></p>

Shows that dissipation and decoherence (reducing $$V$$) are distinct from information storage (increasing $$D$$).

### The Operational Victory

By using the rigorous EGY framework and the MIT team's own analysis, we establish:

1. **Visibility loss ≠ which-way information** (MIT admits this explicitly)
2. **Common-mode detection ≠ path distinguishability** (their $$2D$$ result proves it)
3. **Spectral mixing explains most visibility reduction** (not path knowledge)
4. **Physics papers conflate distinct phenomena** ($$V$$-loss with $$D$$-gain)

This isn't about philosophical interpretations—it's about demanding precision in operational quantities. Most experiments claiming to demonstrate complementarity are actually demonstrating something much less profound: that entanglement and spectral mixing reduce visibility, which has nothing to do with which path light "took" through an apparatus.

The language of "which-way information" has become so imprecise that even leading laboratories publish papers where visibility reduction from spectral mixing is confused with path distinguishability. The EGY framework provides the mathematical tools to cut through this confusion and restore clarity to what these experiments actually measure.
