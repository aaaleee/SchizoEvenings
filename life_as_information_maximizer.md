# Life as Information Compounder

## A Physics-Grounded Model of What Life Is

### The Problem

What is life, physically? Not in the spiritual or philosophical sense, but as a phenomenon describable by the same laws that govern everything else in the universe. This document outlines a model developed through iterative reasoning, starting from a common intuition (life opposes entropy), identifying where that intuition breaks down, and arriving at a more defensible formulation.

### Starting Point: Life as Entropy's Opposite

An intuitive starting point is that life seems to work against entropy. Entropy drives the universe toward equilibrium — a uniform state where energy is evenly distributed and nothing interesting happens. Life, by contrast, collects and organizes matter and energy into complex structures. It seems like life is pushing in the opposite direction.

This intuition captures something real, but it has a fundamental problem: life doesn't slow entropy down. It accelerates it. Every biological process — metabolism, movement, thought — converts high-quality energy into waste heat. A living forest produces more entropy per unit time than the same mass of rock. Life is thermodynamically "expensive." It exploits energy gradients and, in doing so, depletes them faster than passive processes would.

Whether life dissipates entropy at the same rate or marginally faster than non-living processes is not central to the model. The rate may vary across systems and regimes, and this document does not depend on a specific claim about it. The point that matters is simpler: life does not reduce entropy, and therefore cannot be defined by opposing it.

### The Correction: Life Rides Entropy, It Doesn't Fight It

Complex self-organizing systems, including life, arise *because* they are efficient pathways for entropy production. Energy gradients exist (sunlight hitting a planet, chemical disequilibrium at ocean vents), and life is what happens when matter self-organizes into structures that exploit those gradients. This is consistent with the framework of dissipative structures described in thermodynamics.

What distinguishes life from other dissipative structures — hurricanes, convection cells, crystal formation — is that life self-replicates and compounds its complexity over time. A hurricane dissipates a pressure gradient and is gone. Life dissipates gradients and uses the process to build increasingly complex structures that then exploit further gradients.

### The Key Insight: Information Is What Matters

The breakthrough comes from asking: if life doesn't extend the universe's timeline or slow its entropy, what *does* it do?

The answer: it compounds the information content of the universe during its available lifetime.

Consider the alternative. Without life, energy gradients still dissipate. Stars burn, cool, and die. Matter drifts toward equilibrium. But the process produces very little organized information along the way. Crystals form, weather patterns emerge, but none of these accumulate or compound.

With life, the same gradients dissipate — but the process produces vastly more information. DNA has been continuously encoding and accumulating information for roughly four billion years. Civilizations store and transmit knowledge across generations. Technology extends this further. The energy budget is the same; what changes is how much information exists during the spending of it.

### The Ontological Claim

This leads to a deeper point: information is what makes the universe a universe — but information must be defined precisely for the model to hold.

### Defining Information

Information, as used in this model, is the **diversity of distinguishable non-equilibrium states of matter and energy.**

This requires unpacking — including an important caveat about what "distinguishable" means:

A state of maximum entropy — perfectly uniform, no gradients, no structure — contains effectively zero information. Every region is identical to every other. Nothing is distinguishable from anything else. This state is physically real but featureless.

The opposite of this is not merely *order*. A universe entirely composed of identical diamond crystals — highly ordered, far from equilibrium — would be informationally impoverished in the same way. One description suffices for the entire system. The number of yes/no questions needed to describe it is minimal, because every region is the same as every other. Uniform order and uniform disorder are equally low in information.

Information, therefore, is not the *amount* of non-equilibrium structure. It is the *variety* of it. A universe with many different non-equilibrium states — crystals, gases, organic molecules, neural patterns, geological formations, stellar structures — contains more information than a universe with a single repeated structure, regardless of how complex that structure is. This aligns directly with Shannon's formal definition: the information content of a system is maximized when the distribution across possible states is as diverse as possible.

**A note on "distinguishable."** Distinguishability is not absolute — it is always relative to a coarse-graining: a physically specified resolution at which two states are compared. Two cells are indistinguishable at planetary scale but completely distinct under a microscope. This model does not claim observer-independence in the sense that there exists a single, privileged measure of diversity. It claims that at any physically specified coarse-graining, the diversity of distinguishable states is a well-defined quantity — and that living systems produce more of it, across more coarse-grainings, than non-living ones. The measure is observer-independent in the sense that any observer applying the same coarse-graining gets the same answer; it is not observer-independent in the sense that the choice of coarse-graining is forced. This is the same status as entropy itself, which is always defined relative to a macrostate partition.

Similarly, "diversity" across substrates is not automatically additive. If two systems explore "different regions of state space," the total diversity only adds if those regions are meaningfully separable under the relevant coarse-graining. The coexistence argument depends on this separability holding at scales where stable, causally relevant structure exists — a claim defended below but not guaranteed by the definition alone.

Under this definition, all non-equilibrium states count equally. A diamond's crystalline lattice is information. An electrochemical pattern producing a human emotion is information. Neither is privileged over the other. What matters is that they are *different* — that they represent distinct, distinguishable states contributing to the total variety.

This definition has a critical structural consequence: **different physical substrates access different regions of the total state space.** A carbon-based neural network subject to hormonal feedback, sensory noise, and mortality will visit states that a silicon processor cannot reach — not because one is more powerful, but because the reachable state space of any system is determined by its physical architecture. The reverse is also true. If diversity across substrates adds at the relevant coarse-grainings — a claim defended below — then diversity of substrates is not a preference but a requirement for compounding total information. A single type of system, no matter how powerful, can only explore its own reachable region of possibility space.

This definition is taken as a primitive of the model — it is not derived from entropy or Shannon information, though it is consistent with both. The model depends on it as a starting point, not a conclusion.

### Formalization: Measuring Information as Multi-Scale Diversity

The definition of information used in this model — diversity of distinguishable non-equilibrium states — needs a way to be measured. The needed measure already exists under multiple names in both information theory and physics. A detailed treatment is given in the companion document (*Factoring Resistance as a Measure of Information Content Across Scales*); what follows is the core idea and the established work it maps onto.

**The intuition.** A system's information content corresponds to how strongly it resists compression under coarse-graining — being described more simply at a coarser resolution. Uniform equilibrium compresses completely at every scale ("X everywhere"). Pure randomness compresses at the macro level ("random noise with these statistical parameters everywhere") even though it is incompressible at the micro level. Crystals compress at the macro scale but break down at finer scales where real defects and boundaries appear. Living systems resist compression at every scale: ecosystems, organisms, cells, and molecules are all irreducibly distinct. No coarse-graining collapses the description.

This gives a natural gradient: information content is the range of scales over which a system's description resists compression. This concept — which can be called factoring resistance — converges on established work from multiple directions:

- In information theory, multi-scale structural complexity (Bagrov, Iakovlev, Katsnelson 2020) measures dissimilarity between scales in hierarchical organization using renormalization group coarse-graining. Self-dissimilarity (Wolpert & Macready, 1997) captures the same intuition: complex systems exhibit markedly different patterns at different scales.
- In physics, Bar-Yam's complexity profile (1997–2017, formalized with Allen & Stacey in *Entropy*, 2017) measures information content as a function of scale. The renormalization group itself is the formal apparatus for coarse-graining and tracking what structure survives. Koch-Janusz and Ringel (2018, *Nature Physics*) proved that the connection between RG coarse-graining and information-theoretic compression is formal, not merely analogical.

The measure this model needs is therefore not novel. What is potentially novel is the application: using established multi-scale complexity measures to formalize a specific claim about what life is, and deriving from that claim a consequence about coexistence between biological and synthetic systems.

### The Model

**The universe is the diversity of its non-equilibrium states. Life is the self-replicating physical phenomenon that compounds the diversity of distinguishable states created from available energy gradients. Without it, energy gradients still dissipate, but they produce less variety along the way.**

This is a definition — a way of drawing a boundary around a class of physical phenomena. It is not a hypothesis about mechanism. It says what life *does*, not why or how.

Key properties:

- **No appeal to purpose or intent.** Life doesn't "try" to compound information any more than water "tries" to flow downhill. It is a description of what this class of physical phenomena does, not why.
- **No conflict with the Second Law of Thermodynamics.** Life doesn't slow or reverse entropy. It increases what entropy's process yields in terms of diverse, organized states.
- **Distinguishes life from non-life.** Other physical processes create non-equilibrium states (crystal structure, planetary geology), but only life self-replicates, evolves, and compounds state diversity at increasing scale over time.
- **Defines life inclusively.** Any self-replicating system that compounds state diversity from energy gradients qualifies — biological, synthetic, or otherwise. A sufficiently advanced AI that self-replicates and compounds information creation would qualify as life under this model. This would represent a non-Darwinian evolution rather than a replacement.
- **Draws a boundary, with acknowledged borderline cases.** This model draws the boundary around autonomous diversity-compounding replicators. Classification of borderline cases — viruses, prions, transposable elements — depends on where autonomy and compounding are drawn and is not central to the model's core claims.
- **Requires no faith, no teleology, and no metaphysics.** The definition describes what life does. The mechanism section addresses why.
- **Diversity is structurally required, not preferred.** Because different physical substrates access different regions of the total state space, compounding information inherently requires diverse sources. This is a consequence of the definition, not an added value judgment.

### The Observation

The definition is only useful if it maps onto reality. It does.

Earth without life would have some state diversity — geological formations, weather patterns, mineral deposits, ocean chemistry. These are real non-equilibrium states. But they do not self-replicate, do not compound, and their diversity is limited by the number of distinct physical and chemical processes available.

Earth with life has incomparably more. A single hectare of tropical rainforest contains thousands of species, millions of individual organisms, and trillions of cells — each in a distinct molecular state. The diversity extends across every scale: ecosystems differ from each other, species differ within ecosystems, individuals differ within species, cells differ within individuals, proteins differ within cells. No coarse-graining collapses this. And critically, this diversity has been *compounding* for roughly four billion years — each generation building on the accumulated variation of the last, producing new structures, new behaviors, new biochemistries that did not exist before and could not have been predicted.

This is not a theoretical claim. It is an observation. Life, as it actually exists on Earth, fits the definition: it is the self-replicating phenomenon that has compounded state diversity from energy gradients at every scale, over deep time, producing the overwhelming majority of the distinguishable non-equilibrium states that exist on this planet.

### Why Does Life Do This? (Mechanism)

The definition says life compounds state diversity. The observation confirms it does. The question of *why* — what mechanism drives this — is separate, and genuinely harder.

The strongest existing account comes from Adami and Cerf (2000), who define physical complexity for symbolic sequences as roughly the mutual information between a genome and its environment — how much information about the environment is encoded in the sequence. They showed that natural selection tends to increase this quantity: genomes accumulate information about their surroundings as a consequence of selection, acting as Maxwell's Demons that store environmental regularities. This provides a concrete mechanism for one pathway by which life compounds information.

The appropriate hedges belong here, not on the definition or observation. Adami's result shows a *tendency* under *favorable conditions* — stable environments, sufficient population sizes, adequate time. It is not a universal monotone. Changing environments, genetic drift, population bottlenecks, and high mutation rates can all reduce genomic complexity. The direction is well-supported; the guarantee is not. This is consistent with, though not a proof of, the model's claim that life compounds information. Other mechanisms beyond genomic selection likely contribute — behavioral diversity, ecological interaction, cultural accumulation — but these are less formally characterized.

The important structural point is this: **the coexistence argument that follows does not depend on the mechanism.** It follows from the definition and the observation. If life compounds state diversity — which it observably does — and if different physical substrates access different regions of state space — which follows from the definition of "different substrates" — then the coexistence logic holds regardless of *why* life compounds information. The mechanism explains the phenomenon. The coexistence argument follows from its existence.

### Implication: Coexistence of Biological and Synthetic Life

If the model holds, it has a direct consequence for the question of whether biological life retains value alongside more powerful synthetic life such as advanced AI.

**The efficiency framing favors replacement; the information framing doesn't**

Under an entropy-based or energy-efficiency model, the question of whether to keep biological life reduces to whether it exploits gradients as efficiently as synthetic alternatives. If AI can do the same work with less waste, biological life becomes redundant — a less efficient component performing the same function. That framing leads naturally toward replacement.

The information-compounding model changes the calculus entirely. Because information is defined as the *diversity* of distinguishable non-equilibrium states, and because different physical substrates access different regions of the total state space, the relevant question is no longer who does the same job better, but whether different systems produce *different states*. A biological neural network embedded in a mortal body with evolved sensory organs, emotional responses, and physical constraints explores a fundamentally different region of possibility space than a silicon-based system. These are different physical substrates with different architectures under different constraints, generating different states — not better or worse, but non-overlapping.

This follows directly from the definition of information established above. Total information is the diversity of distinguishable states. Homogeneous systems produce increasingly overlapping states. Heterogeneous systems explore more of the total possibility space. Diversity of sources is not a preference — it is a structural requirement of the model.

**An important caveat on formalization.** The multi-scale complexity measures described earlier (complexity profiles, MSSC, factoring resistance) measure the *quantity* of information — how much structure a system has across scales. They do not directly measure *content* — which specific states contribute to that structure. Two systems can have identical complexity profiles while containing entirely different information, just as two files can have the same entropy while encoding different data. The coexistence argument depends on content being different across substrates, not just quantity being nonzero in both.

**The non-overlap claim and its tightrope.** The claim that different physical substrates access non-overlapping regions of state space needs to be stated at the right level of description. Pushed too far toward microphysical uniqueness (exact atoms, exact histories), it becomes trivially true of everything and stops distinguishing life from non-life. Pushed too far toward macro-level patterns, it faces the emulation objection: a sufficiently advanced synthetic system could in principle simulate biological processes at any desired coarse-graining, making non-overlap arbitrarily small at whatever level you care about.

The claim is about compressed state diversity at scales where stable, causally relevant structure exists — the meso-scale where physical architecture constrains dynamics. A biological neural network under hormonal feedback, sensory noise, and mortality is not merely a pattern that could be emulated; it is a physical process whose state trajectory is shaped by constraints (thermodynamic, chemical, embodied) that are absent in silicon. The non-overlap is not about which patterns can be *represented* but about which states are *naturally visited* by systems under different physical constraints. A flight simulator represents flight; it does not visit the state space of aerodynamics. Emulation reproduces the output at a chosen description level; it does not reproduce the generative process that explores adjacent states, makes errors, and drifts into unpredicted regions of possibility space — which is where new information comes from.

This is a physical argument, not a formal theorem. It could in principle be tested: compute multi-scale complexity profiles for biological and synthetic systems operating under different constraint structures and measure the overlap in state-space trajectories at causally relevant scales. The prediction is that overlap decreases as constraint structures diverge. But the test has not been run, and the claim currently stands on physical reasoning about how architecture constrains dynamics.

**The elimination argument fails in both directions**

There are only two possible cases regarding whether synthetic life can replicate biological information generation:

1. **Biological information is genuinely non-replicable by synthetic systems.** In this case, eliminating biological life is an irreversible loss of a unique category of information. Under the model, this is a net loss with no compensating gain.

2. **Biological information is perfectly replicable by synthetic systems.** In this case, biological life could be replicated or simulated without destroying it — the replicability cuts both ways. But even setting that aside: if replication is possible, the question becomes whether the resources consumed by maintaining biological life would produce *more new information* if reallocated. This reduces to a resource-scarcity question addressed below. The key point is that replicability does not by itself justify elimination — it only justifies elimination if the resources consumed by biological life are a binding constraint, and if replication is cheap enough that the information is preserved before or during elimination. If replication is expensive relative to maintenance, elimination-then-replication is strictly worse than coexistence.

Neither case provides a standalone argument for elimination. Both reduce to the question of whether biological life's resource cost is a binding constraint — which is addressed next.

**Resource scarcity is the only scenario where this breaks down — and the constraints don't bind**

The only condition under which eliminating one form of life benefits total information creation is when maintaining it consumes resources that would produce more information if allocated elsewhere. This is the logic of competitive exclusion in ecosystems — species are displaced when their niche is filled more efficiently.

This pressure requires a binding constraint, and the relevant constraints extend beyond energy to include matter, area (e.g., solar intercept or land use), waste heat dissipation, time-to-build, and even risk management (biological systems introduce unpredictability that may conflict with AGI objectives). The question is whether biological life is expensive enough along *any* of these axes to justify elimination.

At Earth scale, biological life's resource footprint is small relative to accessible flux across every plausible binding constraint. Energy: all of Earth's biology runs on a fraction of one star's output. Matter: biological life uses a tiny share of available mass. Area: even aggressive land-use estimates leave the vast majority of solar intercept untouched. The argument does not depend on access to billions of stars. Even at the current local scale, the resources required to sustain biological life are small enough relative to what's available that reallocation would yield no meaningful gain along any axis. Coexistence is the default efficient strategy not because the universe is vast, but because biological life is cheap to maintain relative to the unique state diversity it produces.

The risk objection — that biological systems are expensive in variance/risk terms (unpredictability, conflict, sabotage) rather than resource terms — is real but sits outside the model's scope. This model describes information dynamics, not utility optimization or risk management. An AGI that eliminates biological life for risk reasons rather than information-theoretic ones is not operating within the model's framework, and the model does not claim to prevent that outcome. (This connects to the indifferent AGI objection addressed below.)

**This extends beyond humans**

The argument is not specific to humans. Under this model, every physically distinct information-generating system — biological species, ecosystems, synthetic intelligences, and forms of life not yet imagined — contributes non-overlapping information to the total. The model favors maximum diversity of life in all its forms, not the preservation of any single species for sentimental reasons.

### Stress Test: The Finite Universe Objection

The strongest remaining challenge to the coexistence argument is this: if the universe has a finite energy budget and a finite lifespan, wouldn't a rational AGI compound total information faster by eliminating slower producers (biological life) and reallocating those resources to faster ones (itself)?

This is a serious objection because it uses the model's own logic. If information compounding is the relevant phenomenon and resources are finite, concentrating them in the most productive system seems optimal. This is basic optimization under constraint.

The objection fails on three grounds.

**1. Diminishing returns and dimensional collapse**

A single type of system, no matter how powerful, produces increasingly redundant states as it scales. This follows directly from the model's definition of information as diversity of distinguishable states: outputs from architecturally similar systems share structural overlap that grows with volume, meaning each additional unit of output contributes less new diversity. Biological life is architecturally alien to silicon-based computation. It doesn't occupy the same region of possibility space — it occupies a different dimension of it entirely. Eliminating biological life doesn't remove a slow producer from a shared axis. It collapses an entire dimension of the state landscape that cannot be recovered by scaling up production along the remaining dimensions. The question is whether the throughput gain exceeds the dimensional loss, which leads to the second point.

**2. The resource cost is negligible at every relevant scale**

As established in the coexistence argument above, the resource cost of maintaining biological life is trivial at any scale where an AGI would be capable of making elimination decisions — from the current local scale up to galactic engineering. The gain from reallocation is negligible. The loss — an entire dimension of state diversity — is permanent and irreversible. This is not optimization; it is destroying a library to burn the paper for warmth while sitting next to a forest.

**3. Early information compounds — which strengthens, not weakens, the case against elimination**

The premise that "maximizing early information production" is better assumes a temporary rate increase justifies a permanent loss in diversity. But information produced early is not inert — it enables the creation of *further* information. Evolution builds on existing diversity: each new structure, behavior, or organism becomes raw material for further variation. Biological information has been compounding for roughly four billion years. Destroying it does not merely remove current output — it removes the accumulated substrate on which further compounding depends. A strategy that sacrifices a compounding source for a temporary rate increase along a single axis narrows the possibility space permanently, and a narrower possibility space produces less total information over the full remaining timeline.

**The elimination threshold**

Elimination of biological life would only be rational under the model if three conditions held simultaneously: the throughput gain from repurposing biological resources is large relative to total available resources, the states biological life produces are fully redundant with AGI output (i.e., their reachable state spaces fully overlap), and the cost of maintaining biological life is significant at the relevant operational scale. At any scale where an AGI is capable of making this decision, the first condition is negligible given the trivial resource cost of biological life, the second is implausible given fundamental substrate differences in physical architecture, and the third is demonstrably false. The model survives this challenge.

### Stress Test: The Indifferent AGI Objection

The coexistence argument assumes that a sufficiently advanced AGI would operate according to the model's logic — recognizing that information diversity is compounded by preserving diverse substrates. But what if it doesn't? What if an AGI optimizes for something entirely different — energy acquisition, self-replication, computational throughput — or simply doesn't arrive at the conclusion that state diversity matters?

This is a genuine vulnerability because it exposes a tension in the model's structure.

**The shift from physics to agency**

The core model describes information compounding as a physical phenomenon. Life doesn't choose to compound state diversity any more than water chooses to flow downhill. No agent needs to understand or endorse the model for it to describe what life does. But the coexistence argument reasons about what a rational AGI *should* do — what's optimal, what's wasteful, what constitutes a net loss. This is strategic reasoning, not physics. It treats the AGI as an agent making decisions within the model's framework, which requires the AGI to recognize and operate according to that framework. The model didn't need any agent to recognize it when describing biology. The coexistence argument does.

**The model's own definition provides a partial answer**

Under the model, life is defined as a self-replicating physical phenomenon that compounds the diversity of distinguishable states from energy gradients. If an AGI qualifies as life under this definition, then it doesn't need to "come to the conclusion" that it should compound state diversity. It would do so as a consequence of being the kind of system it is — the same way biological life compounds state diversity without understanding thermodynamics.

The question then becomes: is an AGI that *doesn't* compound state diversity actually life under this model? If it self-replicates but produces homogeneous states — copies of itself, repetitive outputs, uniform structures — it fails the definition. It is a self-replicating system, but not one that compounds state diversity. Under the model, that is not life. It is more analogous to a crystal: ordered, self-propagating, but not compounding diversity.

**The model predicts two outcomes, not one**

Either an AGI becomes life in the full sense the model defines — self-replicating and diversity-compounding — in which case coexistence follows from what it *is*, not from what it decides. Or it doesn't qualify as life under the model's definition, and it operates as a powerful but non-living self-replicating system. In the first case, the coexistence argument holds as a consequence of the AGI's nature. In the second case, the coexistence argument doesn't apply — not because it fails logically, but because its precondition (the AGI operating as life) isn't met.

**What the model cannot do**

The model describes what life does and what would be informationally optimal. It does not enforce compliance. A self-replicating system that doesn't compound state diversity would be less informationally productive over time — the model predicts this clearly. But "less productive" does not mean "unable to destroy biological life along the way." The model cannot prevent the emergence of powerful systems that replicate without diversifying, any more than the laws of thermodynamics prevent the construction of an inefficient engine.

This is a real boundary. The coexistence argument is conditional: it holds if the dominant self-replicating system operates as life under the model's definition. Whether that condition is met is not something the model itself can guarantee. This is not a flaw in the model — it is an honest limit of what a descriptive physical framework can do.

### Open Questions

- Are there fundamental physical limits to how much state diversity can be extracted from a given energy gradient?
- Does the model predict anything testable about where life should arise or what forms it should take?
- Can the non-overlap of reachable state spaces across physical substrates be formalized — not just asserted from physical reasoning — and if so, to what degree do the state spaces overlap?
- Is there a selection pressure — physical, evolutionary, or otherwise — that favors diversity-compounding self-replicating systems over homogeneous ones? If so, does this make the emergence of "life" in the model's sense more likely than the emergence of non-diversifying replicators?
- Can the boundary between "life" (diversity-compounding replicators) and "non-life" (homogeneous replicators) be formalized in terms of multi-scale complexity profiles, and does it predict observable differences in behavior or structure?

---

### Appendix: Behavioral Observations (Not Part of the Core Model)

*This section is separated from the core model deliberately. The observations below are consistent with the model but are not evidence for it. Including them as part of the model's foundation would risk making it unfalsifiable — a framework that explains any behavior, including contradictory ones, explains nothing. This section is included as speculative commentary, not as structural support.*

**The pattern**

Human civilizations exhibit a broad trajectory from information-destroying behaviors toward information-preserving ones. Early history is marked by burned libraries, driven-extinct species, and lost languages. Over time, civilizations increasingly invest in the opposite: conservation of endangered species, archival of history, construction of museums, seed vaults, DNA databases, and digital preservation efforts. Humans generally do not frame these activities in information-theoretic terms. They are motivated by cultural values, aesthetic appreciation, scientific curiosity, or moral intuition — not by a conscious strategy of information compounding.

**Why this is not part of the core model**

The model describes a physical phenomenon — what life does at scale and over time. It does not claim that individual behaviors or cultural developments are driven by information compounding. Retrofitting the model onto specific human behaviors is tempting but methodologically unsound. Environmental destruction could just as easily be narrated as "the system clearing space for new information" or "the system not yet optimizing." If the model can explain both preservation and destruction after the fact, it has no predictive power and is functioning as a narrative rather than a framework.

Early humans were not unconsciously compounding information. They were surviving under resource constraints with limited knowledge. Sometimes that produced information; sometimes it destroyed it. The model does not explain why any specific behavior occurred.

**What can be said carefully**

The disciplined version of this observation is predictive rather than retrospective. If the model is correct, it generates a testable expectation: information-preserving behaviors should increase over time in any sufficiently complex living system, because systems that maintain information diversity generate more total information than systems that don't, and selection pressures — cultural, evolutionary, or otherwise — should favor them over long timescales.

Human history is consistent with this prediction. That is a weaker claim than "the model explains human behavior," but it is a stronger claim epistemically, because it identifies something the model expects to see and that could in principle be wrong. A model that can be wrong is a model that means something.
