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

- A system can be statistically homogeneous at the macro level and still be dynamically rich — meaning its time evolution produces diverse trajectories even if its spatial statistics are uniform. However, as discussed below, time is simply another coarse-graining dimension. A system whose spatial snapshots are factorable but whose spacetime blocks are not would show high factoring resistance when time is included in the partition.
- Macro-level statistical descriptions do not always exhaust macro-level distinguishability. Two regions with identical mean and variance could differ in higher-order correlations, spatial structure, or other features not captured by simple statistical parameters.

These are not fatal objections — in most physically relevant cases, genuine thermodynamic randomness really does collapse distinguishability at the macro level. But the claim should be stated as what it is: a strong tendency with well-understood exceptions, not an absolute law.

For the purposes of the model, the relevant claim is narrower and more defensible: **at thermodynamic equilibrium, randomness factors at the macro level as a physical fact, because equilibrium is defined as the state where no macroscopic measurement can distinguish one region from another.** The overclaim arises only when extending this beyond equilibrium to all random-looking systems, which the model does not require.

---

## Time Is Not a Special Case

An apparent weakness of factoring resistance is that it seems to be a snapshot — a measure of a system's state at a single moment. A frozen crystal with complex defect patterns and a dynamic system could hypothetically have identical spatial F(L) profiles at a given instant. If the measure only captures spatial structure, it cannot distinguish static complexity from dynamic complexity.

This dissolves once you notice that nothing in the definition of factoring resistance restricts it to spatial dimensions.

The procedure is: partition a system into blocks, describe each block, ask whether the descriptions compress. The definition says nothing about those blocks being spatial. If you partition into spacetime blocks — size L in space and T in time — the same operation applies. Partition, describe, compress. The rules do not change. The domain does.

Under spacetime coarse-graining, the frozen crystal factors trivially along the time dimension: "same spatial profile, repeat forever." Its spacetime description compresses to a single spatial snapshot plus a repetition count. A dynamic system whose spatial profile changes over time in non-repeating, non-compressible ways resists factoring in the temporal dimension as well.

This gives a two-parameter profile: F(L, T). L is spatial resolution, T is temporal resolution. The full factoring resistance of a system is its profile across both parameters. A system that resists factoring across spatial scales but not across temporal scales (the frozen crystal) scores lower overall than a system that resists factoring across both.

This is not an extension of the framework. It is the same framework applied to a larger domain. The coarse-graining operation is defined for any partitionable space — and spacetime is partitionable. No new rules, definitions, or exceptions are needed.

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

## Relationship to Existing Work

Factoring resistance was developed independently but converges on concepts that have been formalized from multiple directions in both information theory and physics. This section maps the correspondences. The convergence is treated as validation: independent rediscovery of the same structure from a different starting point confirms that the underlying concept is real, not an artifact of framing.

### Information theory

**Multi-Scale Entropy (MSE) — Costa, Goldberger, Peng (2002).** MSE coarse-grains a time series at scale τ, computes sample entropy at each τ, and plots the resulting curve. Developed for physiological signals to distinguish random noise from structured biological variability. MSE measures unpredictability at each scale independently. Factoring resistance measures compressibility — how much of a description can be reused. MSE treats each scale independently and cannot detect whether structure at one scale predicts structure at another. MSE cannot distinguish scale invariance from scale diversity. Critical noise scores high on MSE at all scales; factoring resistance would score low (statistically compressible). MSE established "complexity ≠ randomness" and "scale matters," but factoring resistance measures something MSE explicitly does not: structural reuse versus irreducible heterogeneity.

**Multi-Scale Structural Complexity (MSSC) — Bagrov, Iakovlev, Katsnelson (2020, PNAS).** Core claim almost verbatim: "Structural complexity of an object is the amount of dissimilarities between distinct scales in its hierarchical organization." Uses multistep renormalization (coarse-graining), computes overlap between neighboring renormalized layers, sums dissimilarities across scales. Designed to be small for both pure order and pure randomness, large for systems with genuinely different structure at different scales. This is factoring resistance. What this document calls "factoring resistance across scales" is their "inter-scale dissimilarity." What this document calls "scale diversity vs scale invariance" is the core distinction MSSC was designed to capture.

**Self-Dissimilarity — Wolpert & Macready (1997, 2007, Santa Fe Institute).** Original formulation: "For systems characterized as complex/living/intelligent, the patterns exhibited on different scales differ markedly from one another. Conversely, the patterns at different scales in simple systems (gases, mountains, crystals) do not vary significantly from one another." MSSC formalized Wolpert and Macready's intuition using RG coarse-graining. Wolpert and Macready explicitly apply their framework to "spatio-temporal densities" — the spacetime extension described earlier in this document was already included in their definition.

### Physics

**Renormalization Group (Wilson, Kadanoff, 1960s-70s).** The entire procedure called "factoring" in this document — partition into blocks, describe, ask what survives — is the renormalization group. Wilson received the Nobel Prize for it. A system at an RG fixed point is scale-invariant (the "scale invariance" case). A system that requires increasingly complex effective descriptions at different scales exhibits "scale diversity." The RG was designed to distinguish exactly these two situations. The RG is not merely analogous to factoring resistance — it is the same operation applied to physical Hamiltonians.

**Complexity Profile — Bar-Yam (1997-2017, NECSI).** The amount of information needed to describe a system as a function of scale. Bar-Yam explicitly developed it as a generalization of RG for complex systems beyond phase transitions. With Allen and Stacey, he formalized it axiomatically in "Multiscale Information Theory and the Marginal Utility of Information" (Entropy, 2017). The F(L) profile defined in this document is a complexity profile viewed through the lens of compression resistance rather than information content. The two framings are likely formally equivalent.

**Effective Complexity — Gell-Mann & Lloyd (1996).** The length of a compressed description of a system's regularities, separating information into a regular part (effective complexity) and a random part (entropy). Both pure order and pure randomness have low effective complexity; complex systems have high. This captures the single-scale version of factoring resistance ("randomness factors, order factors, complexity doesn't") but is not inherently multi-scale.

**Thermodynamic Depth — Lloyd & Pagels (1988).** The difference between a system's coarse-grained and fine-grained entropy. Low for both ordered and random systems, high for complex ones. Measures something different from factoring resistance: how many historical paths could have led to the current state ("how hard was this to build?"), not how much structure exists across scales. Crutchfield and Shalizi (1999) showed it has problems — without a principled way to choose macrostates, the measure is somewhat arbitrary.

**Physical Complexity — Adami & Cerf (2000).** The mutual information between a sequence (such as a genome) and its environment. Adami showed in digital organisms that natural selection forces complexity to increase because genomes act as Maxwell's Demons, storing information about their environment. This is the most biologically grounded physics measure and is directly relevant to the broader model of life as information maximizer that motivates this formalization.

**RSMI (Real-Space Mutual Information) — Koch-Janusz & Ringel (2018, Nature Physics).** The formal proof that RG is information-theoretic compression. Optimal coarse-graining (maximizing mutual information between coarse-grained and fine-grained descriptions) does not increase Hamiltonian complexity — the best compression preserves physical simplicity. Lenggenhager et al. (2020, Phys. Rev. X) extended this to disordered systems. This resolves the open question of whether the RG connection is formal or merely suggestive: it is a theorem.

### What this convergence means

The concept formalized here as factoring resistance has been independently arrived at from statistical physics (RG, complexity profiles), algorithmic information theory (effective complexity, MSSC), and machine learning (RSMI). The core insight — that meaningful complexity is resistance to description-compression under coarse-graining, and that it must be measured across scales — is not novel. It is well-established.

What is established:
- The operation (coarse-graining / partitioning / factoring) has a complete mathematical framework via the RG.
- The connection between RG and information-theoretic compression is proven, not conjectural (Koch-Janusz & Ringel 2018, Lenggenhager et al. 2020).
- The complexity profile (Bar-Yam) provides the multi-scale measure. MSSC (Bagrov et al.) provides the inter-scale dissimilarity measure. Both are computed and applied.
- The distinction between scale invariance and scale diversity is the core of MSSC and self-dissimilarity.
- Physical complexity (Adami) already connects information maximization to biological evolution.

What remains as potential contribution of this document's framing:
- The compression/reuse framing ("how much of this description can be recycled?") may offer computational or conceptual advantages over the dissimilarity framing in specific contexts.
- The spacetime coarse-graining treatment (F(L, T) as a natural two-parameter extension) may be more explicit than in some existing formulations, though Wolpert and Macready already included it implicitly.
- The primary value is in application: using this established mathematical apparatus to formalize a specific claim about what life does and why biological and synthetic systems can coexist. That application is developed in the parent model, not in this document.

---

## Summary of Where Things Stand

**Defined so far:**
- Factoring: compressing a system's description by identifying and replacing repetition (grouping by similarity). Well-defined as an operation. Equivalent to coarse-graining in the renormalization group.
- Scale: coarse-graining resolution L, a continuous physical parameter. Not observer-chosen.
- Factoring resistance F(L): a continuous, graded measure — the residual description length after optimal compression at resolution L. Not binary. Corresponds to the complexity profile (Bar-Yam) and inter-scale dissimilarity (MSSC).
- Total factoring resistance: the profile of F(L) across all accessible L. Maximum information corresponds to systems where F(L) remains high across the full range.
- Spacetime extension: time is another coarse-graining dimension, giving F(L, T). No new rules required. Static systems factor along T; dynamic systems may not.
- Maximality: a property of the F(L) profile, not a scalar. Can be partial ("maximal between L₁ and L₂"). Equal profiles mean equal quantity of information, not equal content.
- RG connection: proven formal, not merely suggestive (Koch-Janusz & Ringel 2018). The full mathematical apparatus of RG theory is available.

**Not yet defined in this document (but may exist in the literature):**
- The precise metric for "residual description length." Multiple candidates exist (Shannon entropy of the block-description distribution, normalized compression distance, mutual information between blocks). MSSC uses overlap between renormalized layers. The complexity profile uses Shannon information. The right choice may depend on context.
- The formal distinction between scale invariance and scale diversity. MSSC and self-dissimilarity address this directly but the mapping to the compression framing used here has not been made explicit.
