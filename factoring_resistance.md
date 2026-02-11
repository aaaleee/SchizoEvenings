# Factoring Resistance: Toward a Formal Measure of Information Content

*Working document. This explores the formalization of "factoring resistance" — the idea that information is what resists factoring, and that maximum information is a state that resists factoring at every scale. This document attempts to make that concept rigorous.*

---

## The Problem

The claim is:

**Information is what resists factoring. Maximum information is a state that resists factoring at every accessible scale of description.**

This is intuitive. A sequence (A,B,B,B,C,C) factors to A + 3B + 2C. The sequence (C,B,F,P,E) does not factor — every element must be stated. Applied to physical systems: a uniform cosmos factors at every scale, a crystal factors at macro but not micro, a living universe resists factoring at every scale.

The problem is that "factoring" and "scale" are doing all the work, and neither is formally defined. A hostile but competent critic will ask:

- Factoring with respect to what algebra? What operations are allowed?
- Under what transformations? Can you rotate, permute, relabel?
- What counts as a "scale" — and who chooses the scales?

Without answers, factoring resistance risks becoming "looks irreducibly complex at all resolutions we care about" — which reintroduces exactly the observer-dependence it was designed to eliminate. The concept would not be logically unfalsifiable, but it would be operationally unfalsifiable, which is nearly as bad.

This document works toward answering those questions — or at least narrowing them to the point where formal treatment becomes possible.

---

## What "Factoring" Means

### The intuition

Factoring, as used here, means: reducing a description by identifying and compressing repetition. If parts of a system are identical or statistically indistinguishable, the description can be shortened by replacing them with a count and a template. "1000 identical crystals" is shorter than listing each one. "Random noise with mean μ and variance σ" is shorter than listing each value.

A system resists factoring when no such reduction is available — when the description cannot be shortened without losing information about the system's actual state.

### What algebra?

The factoring operations are not arbitrary. They correspond to a specific class of transformations: **partitioning a system into regions and testing whether those regions can be described by a shared template plus a count (or a shared statistical distribution plus parameters).**

More precisely:

1. Choose a partition of the system into regions.
2. For each region, produce a description at the chosen resolution.
3. Ask: can the set of region-descriptions be compressed? That is, can many of them be replaced by a reference to a shared description?

If yes, the system factors under that partition. If no partition at that resolution allows compression, the system resists factoring at that scale.

But compression is not binary. Almost no physical system will cleanly "factor" or "not factor" — there are degrees. A description might be reducible by 90%, or by 5%, or by 0.01%. If factoring resistance is treated as binary — either it factors or it doesn't — then the concept becomes brittle. A threshold would be needed, and that threshold would be an arbitrary choice.

The correct commitment is: **F(L) is a continuous, graded measure.** At each scale L, factoring resistance is the residual description length after optimal compression — how much of the description survives once all repetition has been removed. A crystal at the macro level has near-zero residual. A random system at the macro level also has near-zero residual (its statistics compress to a few parameters). A system with genuinely diverse structure resists compression, leaving a high residual.

This means F(L) is not a predicate ("factors" vs "doesn't factor") but a quantity. Systems can be compared. Factoring resistance can increase or decrease. The concept survives contact with real systems where nothing is perfectly compressible or perfectly incompressible.

This does not discard the binary concept — it subsumes it. F(L) ranges from zero (fully compressible) to a maximum (nothing compresses). If a system hits that maximum at a given L — every region's description is irreducibly unique, no compression is possible — then it is fully resistant at that scale. That is a binary fact. Full resistance is the upper bound of the continuous measure, not a separate concept.

This is not a free-form algebra. The allowed operation is specifically: grouping and compressing by similarity. This is well-defined and does not depend on an observer's preferences — two descriptions either are or are not statistically distinguishable, as a matter of physical fact.

### What counts as "identical" or "indistinguishable"?

Two region-descriptions are identical if they specify the same physical state. They are statistically indistinguishable if no measurement at the given resolution could reliably distinguish them. This is an operational definition grounded in physics, not in observer choice — it corresponds to asking whether two regions would produce different outcomes in a physical experiment at the relevant resolution. Because F(L) is defined in terms of the complete description at resolution L — everything the physics contains at that scale, not a chosen subset of observables — there is no menu of measurements to select from. The only parameter is L itself, which is a continuous physical quantity, not an observer decision.

---

## What "Scale" Means

This is the harder question. If "resists factoring at every scale" is the definition, then "scale" must be defined without an observer choosing it.

### Coarse-graining: a physics-native definition of scale

Physics already has a standard framework for this: **coarse-graining**.

Take a physical system and impose a resolution length L. At resolution L, you cannot distinguish features smaller than L — they are averaged over, smoothed out, or described only statistically. As L varies from the smallest physically meaningful length up to the size of the entire system, you get a continuous family of descriptions at different resolutions.

At each L:

- Partition the system into cells of size L.
- Describe each cell at resolution L (its average density, composition, temperature, or whatever quantities are relevant).
- Ask: can the resulting set of cell-descriptions be compressed?

This defines factoring resistance as a function of L — call it F(L). The system's total factoring resistance is the profile of F across all L.

**This is not observer-chosen.** The coarse-graining parameter L is a physical length, not a subjective decision. It corresponds to the resolution of a measurement apparatus — and the question "are two cells distinguishable at resolution L?" has a definite physical answer for any given L.

### Continuous or discrete?

The coarse-graining parameter L is continuous in principle. In practice, many physical systems have natural scales where structure is concentrated — atomic, molecular, cellular, organismal, ecological. Between these scales, the factoring resistance profile might be relatively flat, with sharp changes at the transitions.

This suggests that for real physical systems, a discrete set of "important scales" may emerge from the continuous profile — not because the definition requires discreteness, but because the physics produces it. The formalism should be continuous, with the discrete scales being a feature of specific systems, not of the definition itself.

### Connection to renormalization group theory

This framework has a deep connection to the **renormalization group** (RG) in physics.

The renormalization group studies exactly this question: how does a system's description change as you vary the resolution scale? Systems at critical points (phase transitions) are the ones where non-trivial structure persists at every scale — they are scale-invariant, meaning no coarse-graining resolution gives you a simpler description.

This is suggestive. In the language of factoring resistance:

- A system far from criticality factors at most scales (it has a characteristic length scale, and beyond that scale, it is uniform).
- A system at a critical point resists factoring at every scale (structure is present at all resolutions).

This parallel must be stated carefully.

**Scale invariance is not scale diversity.** A critical system — like a fluid at its boiling point or a magnet at its Curie temperature — resists simplification across scales. But it is often statistically self-similar: the same kind of structure repeats at every resolution. A critical Ising model has fluctuations at every scale, but those fluctuations are governed by the same statistical law everywhere. Under the graded definition of F(L), such a system might still have relatively low factoring resistance, because the description at each scale can be compressed to: "same statistical law, different realization." The structure persists, but it factors statistically.

The distinction that matters for factoring resistance is between:

- **Scale invariance:** non-trivial structure at every scale, but self-similar (same type of structure repeated). May still compress statistically.
- **Scale diversity:** genuinely different kinds of structure at different scales, where the description at one scale does not predict the description at another.

Maximum factoring resistance requires scale diversity, not merely scale invariance. A turbulent fluid or a critical system resists coarse-graining, but if its structure at every scale is governed by the same statistical law, its cross-scale description still compresses. A system with qualitatively different organization at different scales — where molecular-level structure is unlike macro-level structure, which is unlike large-scale structure — resists this compression.

This distinction is present in the concept but not yet formalized. A critic armed with turbulence, strange attractors, or critical systems can legitimately demand: "Show me why these score lower on F(L) than a scale-diverse system." The answer must come from the graded measure, not from hand-waving about what "feels" more complex.

The formal tools of the renormalization group (RG flow, fixed points, scaling exponents) might provide a useful mathematical framework for defining and computing factoring resistance. This is a candidate formalization pathway, not a claimed result.

---

## A Concrete Example

To test whether factoring resistance is a real, measurable property rather than a hand-wave, consider three cities viewed at different zoom levels. The "zooming" is exactly what coarse-graining does — changing the resolution at which you describe the system.

**The Uniform City.** Every district is identical. Zoom into a district — every block is identical. Zoom into a block — every building is identical. Zoom into a building — every room is identical. At every zoom level, you see one thing repeated. "Copy-paste at every zoom" is the total description. This city factors completely at every scale. F(L) = 0 everywhere.

**The Random City.** Buildings of random shapes, sizes, and colors scattered everywhere with no pattern. At street level, every building is unique — you cannot factor the description. But zoom out to the neighborhood level, and every neighborhood has the same statistical mix of random buildings. Zoom out to the district level — identical statistics again. From above, the randomness looks the same everywhere. This city factors at every macro zoom level, despite micro-level uniqueness. F(L) is high only at the finest zoom, then drops.

**The Living City.** Districts are distinct from each other — a financial district, a market quarter, a residential area, an arts district. Zoom into a district — blocks differ from each other. Zoom into a block — buildings differ. Zoom into a building — rooms differ. At every zoom level, you are seeing something you could not have predicted from any other part of the city. No zoom level gives you a shortcut. This city resists factoring at every scale. F(L) remains high across the full range of zoom levels.

The parallel to the three canonical cases is direct. The Uniform City is the crystal — compressible at every scale. The Random City is the uniform noise — micro-level diversity but macro-level sameness. The Living City is the scale-diverse system — irreducible structure at every resolution.

**What "computing F(L)" would mean here:**

At each zoom level:
1. Divide the city into regions of that size (rooms, buildings, blocks, neighborhoods, districts).
2. Describe each region at that resolution.
3. Ask: how many of these descriptions are interchangeable? Can the set be compressed?

If most regions are interchangeable (Uniform City), compression is easy — low F. If regions are statistically identical despite individual variation (Random City), compression is still possible at that scale — low F. If regions are genuinely distinct and no compression works (Living City), F is high.

This is measurable. It is not the final formalization — real physical systems are more complex than cities — but it demonstrates that factoring resistance across scales is a concrete, testable property, not a philosophical abstraction.

**A note on the city analogy:** The example presents scales as discrete and given — rooms, buildings, blocks, districts. This is a feature of cities, not of the definition. In a physical system, the coarse-graining parameter L is continuous. You can set L to any value, and the description at that resolution is well-defined — you are asking "what does the system look like when everything below this resolution is blurred out?" The discrete scales that appear in the city example are not inputs to the method. In a real system, they would be outputs — features discovered by sweeping L continuously and seeing where the F(L) profile shows structure. You don't choose the scales. The system tells you where they are.

---

## The Randomness Claim, Revisited

The earlier sections of this document state that randomness "factors perfectly at the macro level." This is a useful intuition but slightly too strong.

The more defensible claim is: **randomness collapses macro-level distinguishability, even when micro-level states differ.**

The distinction matters because:

- A system can be statistically homogeneous at the macro level and still be dynamically rich — meaning its time evolution produces diverse trajectories even if its spatial statistics are uniform. Factoring resistance as defined here is a snapshot measure. A system that looks factorable at every scale at any given moment might produce unfactorable sequences over time.
- Macro-level statistical descriptions do not always exhaust macro-level distinguishability. Two regions with identical mean and variance could differ in higher-order correlations, spatial structure, or other features not captured by simple statistical parameters.

These are not fatal objections — in most physically relevant cases, genuine thermodynamic randomness really does collapse distinguishability at the macro level. But the claim should be stated as what it is: a strong tendency with well-understood exceptions, not an absolute law.

For the purposes of the model, the relevant claim is narrower and more defensible: **at thermodynamic equilibrium, randomness factors at the macro level as a physical fact, because equilibrium is defined as the state where no macroscopic measurement can distinguish one region from another.** The overclaim arises only when extending this beyond equilibrium to all random-looking systems, which the model does not require.

---

## What "Maximum Information" Means

Once F(L) is defined as a graded, continuous function of scale, "maximum information" needs to be stated precisely — and the answer is less obvious than it first appears.

### Maximality is a profile, not a number

The natural instinct is to treat total information as a scalar — sum or integrate F(L) across all scales and get a single number. But this loses most of what F(L) captures. Two systems with the same integrated F could have radically different profiles: one might have high factoring resistance concentrated at fine scales (like randomness), another might have it concentrated at coarse scales, and a third might have moderate resistance spread across all scales.

The more precise statement: **maximum information corresponds to a system whose F(L) profile remains high across the full accessible range of L.** Information is not a volume — it is coverage of scale space. A system is maximally informative not when it scores highest on a single number, but when it resists factoring broadly, at many scales simultaneously.

This means maximality can be partial and localized. A system can be "maximal between L₁ and L₂" — meaning its factoring resistance is saturated over that range of scales but not others. This is more precise, more physical, and more useful than a single scalar.

### Equal quantity is not equal content

A consequence: two systems can have the same F(L) profile — the same quantity of information — while containing entirely different information. This is not a flaw. Physics already works this way. Two systems can have the same entropy but radically different microstates. Two signals can have the same Shannon entropy but encode entirely different messages.

Under this framework:

- **Quantity of information** = the F(L) profile (how much factoring resistance, distributed across which scales).
- **Content of information** = which specific states are present (what the irreducible descriptions actually say).

Two maximally informative systems are informationally equal in quantity but potentially non-overlapping in content.

### Comparison and ranking

If maximality is a profile rather than a scalar, then ranking systems requires care. Two systems that are both maximal across the same range of L cannot be ranked — they are informationally equivalent in quantity, differing only in content. Ranking only makes sense when comparing systems with different profiles: one that is maximal across more of the scale range contains more information than one that is maximal across less.

This is not a weakness — it is a design choice that reflects the structure of the concept. Attempting to force a total ordering where the concept supports only a partial ordering would be false precision.

### Saturation is inevitable

If information is coverage of scale space, there is a ceiling. The universe has finite energy, which means finite degrees of freedom, which means a finite number of distinguishable states. The F(L) profile cannot grow indefinitely — there is a physical maximum set by the energy budget of the system.

This is not speculative. It is a direct consequence of thermodynamics and is formalized in physics as the Bekenstein bound, which puts a hard upper limit on the information content of any finite region with finite energy.

The consequence for any system approaching saturation: once the F(L) profile is maximal across all accessible scales, no further increase is possible — only substitution. New states can replace existing ones, but the total quantity of information cannot grow. The system transitions from *increasing* its information to *diversifying within the ceiling* — replacing content, turning over configurations, exploring different states within the same total capacity.

This is a prediction of the framework, not a weakness. It says that information growth in any finite system has a physical endpoint, and that beyond that point, change continues but growth does not. Whether this transition is observable on any practical timescale is a separate question — but the ceiling itself is a fact of physics.

---

## Summary of Where Things Stand

**Defined so far:**
- Factoring: compressing a system's description by identifying and replacing repetition (grouping by similarity). Well-defined as an operation.
- Scale: coarse-graining resolution L, a continuous physical parameter. Not observer-chosen.
- Factoring resistance F(L): a continuous, graded measure — the residual description length after optimal compression at resolution L. Not binary.
- Total factoring resistance: the profile of F(L) across all accessible L. Maximum information corresponds to systems where F(L) remains high across the full range.
- Maximality: a property of the F(L) profile, not a scalar. Can be partial ("maximal between L₁ and L₂"). Equal profiles mean equal quantity of information, not equal content.

**Not yet defined:**
- The precise metric for "residual description length." Multiple candidates exist (Shannon entropy of the block-description distribution, normalized compression distance, mutual information between blocks). The right choice may depend on context or may require a new definition.
- How to handle temporal structure. The current framework is spatial — it asks whether a system's state at a given moment resists factoring. A temporal extension — factoring resistance of the system's trajectory through state space — is needed but not yet formulated.
- Whether the renormalization group connection is formal or merely suggestive. If factoring resistance can be mapped onto RG concepts, the entire mathematical apparatus of RG theory becomes available. If not, a new formalism is needed.
- The formal distinction between scale invariance (self-similar structure at every scale, compressible statistically) and scale diversity (qualitatively different structure at different scales, not statistically compressible). This distinction is conceptually clear but not yet captured by F(L) without additional machinery.

**Open questions for this document:**
- Is there a natural way to extend factoring resistance to temporal sequences — a system's history, not just its current state?
- Does the RG connection hold formally, or is it an analogy?
- What is the right compressibility metric, and does the choice matter (i.e., do different metrics give qualitatively different results)?
- Can factoring resistance formally distinguish between scale invariance (turbulence, critical systems) and scale diversity? If so, what mathematical property separates them?
- Can F(L) be computed for a concrete system before and after a new class of states is introduced, and does the profile shift upward as expected?
- Given that any finite system has an information ceiling, what does the transition from growth to turnover look like in the F(L) profile — and is it observable or only theoretical?
