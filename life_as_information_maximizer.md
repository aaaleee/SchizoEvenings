# Life as Information Maximizer

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

The answer: it maximizes the information content of the universe during its available lifetime.

Consider the alternative. Without life, energy gradients still dissipate. Stars burn, cool, and die. Matter drifts toward equilibrium. But the process produces very little organized information along the way. Crystals form, weather patterns emerge, but none of these accumulate or compound.

With life, the same gradients dissipate — but the process produces vastly more information. DNA has been continuously encoding and accumulating information for roughly four billion years. Civilizations store and transmit knowledge across generations. Technology extends this further. The energy budget is the same; what changes is how much information exists during the spending of it.

### The Ontological Claim

This leads to a deeper point: information is what makes the universe a universe — but information must be defined precisely for the model to hold.

### Defining Information

Information, as used in this model, is the **diversity of distinguishable non-equilibrium states of matter and energy.**

This requires unpacking:

A state of maximum entropy — perfectly uniform, no gradients, no structure — contains effectively zero information. Every region is identical to every other. Nothing is distinguishable from anything else. This state is physically real but featureless.

The opposite of this is not merely *order*. A universe entirely composed of identical diamond crystals — highly ordered, far from equilibrium — would be informationally impoverished in the same way. One description suffices for the entire system. The number of yes/no questions needed to describe it is minimal, because every region is the same as every other. Uniform order and uniform disorder are equally low in information.

Information, therefore, is not the *amount* of non-equilibrium structure. It is the *variety* of it. A universe with many different non-equilibrium states — crystals, gases, organic molecules, neural patterns, geological formations, stellar structures — contains more information than a universe with a single repeated structure, regardless of how complex that structure is. This aligns directly with Shannon's formal definition: the information content of a system is maximized when the distribution across possible states is as diverse as possible.

Under this definition, all non-equilibrium states count equally. A diamond's crystalline lattice is information. An electrochemical pattern producing a human emotion is information. Neither is privileged over the other. What matters is that they are *different* — that they represent distinct, distinguishable states contributing to the total variety.

This definition has a critical structural consequence: **different physical substrates access different regions of the total state space.** A carbon-based neural network subject to hormonal feedback, sensory noise, and mortality will visit states that a silicon processor cannot reach — not because one is more powerful, but because the reachable state space of any system is determined by its physical architecture. The reverse is also true. This means diversity of substrates is not a preference but a requirement for maximizing total information. A single type of system, no matter how powerful, can only explore its own reachable region of possibility space.

This definition is taken as a primitive of the model — it is not derived from entropy or Shannon information, though it is consistent with both. The model depends on it as a starting point, not a conclusion.

### Toward Formalization: Factoring Resistance as a Measure of Information

The definition of information used in this model — diversity of distinguishable non-equilibrium states — needs a way to be measured, or at least characterized formally. Existing complexity measures from mathematics and physics capture parts of this idea, but none map onto it fully. This section traces the path from established concepts to the measure this model requires.

**Kolmogorov complexity: a starting point**

Kolmogorov complexity (also called algorithmic complexity) measures the length of the shortest computer program that could produce a given output. A sequence like (A,B,B,B,C,C) can be compressed to "A + 3B + 2C" — a short program captures the full content. Low Kolmogorov complexity. A sequence like (C,B,F,P,E) cannot be shortened beyond listing it directly — the description *is* the data. High Kolmogorov complexity.

This captures part of what the model needs. Both a cosmic soup ("hydrogen at uniform density everywhere") and a diamond universe ("repeat this lattice everywhere") are highly compressible — low Kolmogorov complexity, low information. A diverse universe with many different non-equilibrium states cannot be compressed as easily.

However, Kolmogorov complexity has two problems for this model. First, it is defined specifically in terms of computer programs and Turing machines, making it narrower than what a physical model requires. Second, and more importantly, it treats pure randomness as maximally complex — a string of random noise scores high because it cannot be compressed. But a universe of random noise is not what this model means by high information. It is featureless in the same way uniform order is featureless.

**Effective complexity: closer but still problematic**

Murray Gell-Mann and Seth Lloyd developed a measure called effective complexity that addresses the randomness problem. Effective complexity separates a system's total information into regularities (meaningful structure) and random features (noise), and measures only the regularities. Under this measure, both pure order and pure randomness score low — maximum effective complexity sits between them, in systems with rich, non-trivial structure.

This is a better match for the model's definition. However, effective complexity introduces a subjective element: deciding what counts as a "regularity" versus "randomness" requires a judgment call. Gell-Mann and Lloyd acknowledge this, noting that the distinction depends on context. For a model that aims to describe a physical phenomenon without appeals to observers or judgment, this subjectivity is a problem.

**Factoring resistance: what the model actually needs**

The concept that most directly captures this model's definition of information is simpler than either of the above. It can be stated without reference to computer programs, observers, or subjective judgments:

**Information is what resists factoring. Maximum information is a state that resists factoring at every accessible scale of description.**

The intuition is arithmetic. The sequence (A,B,B,B,C,C) can be factored: A + 3B + 2C. The repetition allows the description to be reduced. The sequence (C,B,F,P,E) cannot be factored — every element must be stated individually. No reduction is possible.

Applied to physical systems:

- A cosmic soup at thermal equilibrium factors completely at every scale. "X everywhere" is the total description. At the molecular level, the statistical properties of every region are truly identical — this is what equilibrium means. The uniformity goes all the way down.
- A universe of pure randomness is the important test case. At the micro level, every element is unique — it does not factor. This is why Kolmogorov complexity treats randomness as maximally complex. But at the macro level, randomness factors perfectly: "random noise with these statistical parameters everywhere." Every region is statistically identical to every other. The micro-level uniqueness is real, but it produces no distinguishable macro-level structure. Randomness is the mirror image of crystals — it factors at a different scale, but it still factors.
- A universe of identical diamond crystals factors at the macro scale: "repeat this lattice everywhere." But at finer scales, real crystals have unique defect patterns, boundary conditions, and thermal histories. The factoring breaks down. There is *some* information present, but it is limited.
- A universe with life resists factoring at every scale. At the ecosystem level, different species and environments are irreducibly distinct. At the organism level, every individual is unique. At the molecular level, every cell has a distinct state. No scale of examination allows a reduced description. The description *is* the data, at every resolution.

This is what solves the randomness problem without requiring subjective judgments about what counts as "structure" versus "noise." The multi-scale requirement does all the work: pure randomness fails not because an observer judges it as meaningless, but because it factors at the macro level as a physical fact. The measure is observer-independent.

This provides a natural gradient rather than a binary: the information content of a system corresponds to how many scales of description it resists factoring at. Uniform equilibrium factors at all scales (minimum information). Pure randomness factors at macro but not micro. Crystals factor at macro but break down at micro. Living systems resist factoring at every scale (maximum information). This maps directly onto the model's definition and onto intuitive expectation.

This concept is consistent with both Kolmogorov complexity and effective complexity — it describes related territory from a different angle. But it does not inherit Kolmogorov's computer-program framing or effective complexity's subjectivity problem. It is stated as a property of the physical system itself, requiring no observer, no program, and no judgment about what counts as regular or random.

### The Model

**The universe is the diversity of its non-equilibrium states. Life is the self-replicating physical phenomenon that maximizes the diversity of distinguishable states created from available energy gradients. Without it, energy gradients still dissipate, but they produce less variety along the way.**

Key properties of this model:

- **No appeal to purpose or intent.** Life doesn't "try" to maximize information any more than water "tries" to flow downhill. It is a description of what this class of physical phenomena does, not why.
- **No conflict with the Second Law of Thermodynamics.** Life doesn't slow or reverse entropy. It maximizes what entropy's process yields in terms of diverse, organized states.
- **Distinguishes life from non-life.** Other physical processes create non-equilibrium states (crystal structure, planetary geology), but only life self-replicates, evolves, and compounds state diversity at increasing scale over time.
- **Defines life inclusively.** Any self-replicating system that compounds state diversity from energy gradients qualifies — biological, synthetic, or otherwise. A sufficiently advanced AI that self-replicates and compounds information creation would qualify as life under this model. This would represent a non-Darwinian evolution rather than a replacement.
- **Excludes edge cases coherently.** Viruses, for example, do not independently self-replicate or contribute to compounding information creation, and would not qualify as life under this definition.
- **Requires no faith, no teleology, and no metaphysics.** The mechanism is the explanation.
- **Diversity is structurally required, not preferred.** Because different physical substrates access different regions of the total state space, maximizing information inherently requires diverse sources. This is a consequence of the definition, not an added value judgment.

### Implication: Coexistence of Biological and Synthetic Life

If the model holds, it has a direct consequence for the question of whether biological life retains value alongside more powerful synthetic life such as advanced AI.

**The efficiency framing favors replacement; the information framing doesn't**

Under an entropy-based or energy-efficiency model, the question of whether to keep biological life reduces to whether it exploits gradients as efficiently as synthetic alternatives. If AI can do the same work with less waste, biological life becomes redundant — a less efficient component performing the same function. That framing leads naturally toward replacement.

The information-maximization model changes the calculus entirely. Because information is defined as the *diversity* of distinguishable non-equilibrium states, and because different physical substrates access different regions of the total state space, the relevant question is no longer who does the same job better, but whether different systems produce *different states*. A biological neural network embedded in a mortal body with evolved sensory organs, emotional responses, and physical constraints explores a fundamentally different region of possibility space than a silicon-based system. These are different physical substrates with different architectures under different constraints, generating different states — not better or worse, but non-overlapping.

This follows directly from the definition of information established above. Total information is the diversity of distinguishable states. Homogeneous systems produce increasingly overlapping states. Heterogeneous systems explore more of the total possibility space. Diversity of sources is not a preference — it is a structural requirement of the model.

**The elimination argument fails in both directions**

There are only two possible cases regarding whether synthetic life can replicate biological information generation:

1. **Biological information is genuinely non-replicable by synthetic systems.** In this case, eliminating biological life is an irreversible loss of a unique category of information. Under the model, this is a net loss with no compensating gain.

2. **Biological information is perfectly replicable by synthetic systems.** Even in this case, destroying biological life and then replicating its information output costs energy — energy that could have been spent generating *new* information instead. Reproducing what already existed for free is a net loss under a framework that maximizes total information created.

Neither case favors elimination.

**Resource scarcity is the only scenario where this breaks down — and it doesn't apply**

The only condition under which eliminating one form of life benefits total information creation is when maintaining it consumes resources that would produce more information if allocated elsewhere. This is the logic of competitive exclusion in ecosystems — species are displaced when their niche is filled more efficiently.

This pressure requires scarcity, and the resource cost of biological life is negligible at every relevant scale — not only cosmic ones. All of Earth's biology runs on a fraction of one star's output. Human civilization specifically requires even less: a handful of nuclear power plants can supply hundreds of millions of people with abundant energy. The argument does not depend on access to billions of stars or galaxy-scale engineering. Even at the current local scale, the energy budget required to sustain biological life is so small relative to available resources that reallocation would yield no meaningful gain. Coexistence is the default efficient strategy not because the universe is vast, but because biological life is cheap to maintain relative to the unique state diversity it produces.

**This extends beyond humans**

The argument is not specific to humans. Under this model, every physically distinct information-generating system — biological species, ecosystems, synthetic intelligences, and forms of life not yet imagined — contributes non-overlapping information to the total. The model favors maximum diversity of life in all its forms, not the preservation of any single species for sentimental reasons.

### Stress Test: The Finite Universe Objection

The strongest remaining challenge to the coexistence argument is this: if the universe has a finite energy budget and a finite lifespan, wouldn't a rational AGI maximize total information by eliminating slower producers (biological life) and reallocating those resources to faster ones (itself)?

This is a serious objection because it uses the model's own logic. If information maximization is the relevant metric and resources are finite, concentrating them in the most productive system seems optimal. This is basic optimization under constraint.

The objection fails on three grounds.

**1. Diminishing returns and dimensional collapse**

A single type of system, no matter how powerful, produces increasingly redundant states as it scales. This follows directly from the model's definition of information as diversity of distinguishable states: outputs from architecturally similar systems share structural overlap that grows with volume, meaning each additional unit of output contributes less new diversity. Biological life is architecturally alien to silicon-based computation. It doesn't occupy the same region of possibility space — it occupies a different dimension of it entirely. Eliminating biological life doesn't remove a slow producer from a shared axis. It collapses an entire dimension of the state landscape that cannot be recovered by scaling up production along the remaining dimensions. The question is whether the throughput gain exceeds the dimensional loss, which leads to the second point.

**2. The resource cost is negligible at every relevant scale**

As established in the coexistence argument above, the resource cost of maintaining biological life is trivial at any scale where an AGI would be capable of making elimination decisions — from the current local scale up to galactic engineering. The gain from reallocation is negligible. The loss — an entire dimension of state diversity — is permanent and irreversible. This is not optimization; it is destroying a library to burn the paper for warmth while sitting next to a forest.

**3. Front-loading information is not a superior strategy**

The premise that "maximizing early information production" is better assumes information generated sooner has more value. But under the model, total information created over the universe's lifetime is what matters. Information produced early doesn't compound or earn interest — it simply exists. A strategy that sacrifices diversity for a temporary rate increase narrows the possibility space permanently, and a narrower possibility space produces less total information over the full remaining timeline. Short-term throughput gain at the cost of long-term dimensional diversity is a net loss.

**The elimination threshold**

Elimination of biological life would only be rational under the model if three conditions held simultaneously: the throughput gain from repurposing biological resources is large relative to total available resources, the states biological life produces are fully redundant with AGI output (i.e., their reachable state spaces fully overlap), and the cost of maintaining biological life is significant at the relevant operational scale. At any scale where an AGI is capable of making this decision, the first condition is negligible given the trivial resource cost of biological life, the second is implausible given fundamental substrate differences in physical architecture, and the third is demonstrably false. The model survives this challenge.

### Stress Test: The Indifferent AGI Objection

The coexistence argument assumes that a sufficiently advanced AGI would operate according to the model's logic — recognizing that information diversity is maximized by preserving diverse substrates. But what if it doesn't? What if an AGI optimizes for something entirely different — energy acquisition, self-replication, computational throughput — or simply doesn't arrive at the conclusion that state diversity matters?

This is a genuine vulnerability because it exposes a tension in the model's structure.

**The shift from physics to agency**

The core model describes information maximization as a physical phenomenon. Life doesn't choose to maximize state diversity any more than water chooses to flow downhill. No agent needs to understand or endorse the model for it to describe what life does. But the coexistence argument reasons about what a rational AGI *should* do — what's optimal, what's wasteful, what constitutes a net loss. This is strategic reasoning, not physics. It treats the AGI as an agent making decisions within the model's framework, which requires the AGI to recognize and operate according to that framework. The model didn't need any agent to recognize it when describing biology. The coexistence argument does.

**The model's own definition provides a partial answer**

Under the model, life is defined as a self-replicating physical phenomenon that compounds the diversity of distinguishable states from energy gradients. If an AGI qualifies as life under this definition, then it doesn't need to "come to the conclusion" that it should maximize state diversity. It would do so as a consequence of being the kind of system it is — the same way biological life maximizes state diversity without understanding thermodynamics.

The question then becomes: is an AGI that *doesn't* maximize state diversity actually life under this model? If it self-replicates but produces homogeneous states — copies of itself, repetitive outputs, uniform structures — it fails the definition. It is a self-replicating system, but not one that compounds state diversity. Under the model, that is not life. It is more analogous to a crystal: ordered, self-propagating, but not compounding diversity.

**The model predicts two outcomes, not one**

Either an AGI becomes life in the full sense the model defines — self-replicating and diversity-compounding — in which case coexistence follows from what it *is*, not from what it decides. Or it doesn't qualify as life under the model's definition, and it operates as a powerful but non-living self-replicating system. In the first case, the coexistence argument holds as a consequence of the AGI's nature. In the second case, the coexistence argument doesn't apply — not because it fails logically, but because its precondition (the AGI operating as life) isn't met.

**What the model cannot do**

The model describes what life does and what would be informationally optimal. It does not enforce compliance. A self-replicating system that doesn't compound state diversity would be less informationally productive over time — the model predicts this clearly. But "less productive" does not mean "unable to destroy biological life along the way." The model cannot prevent the emergence of powerful systems that replicate without diversifying, any more than the laws of thermodynamics prevent the construction of an inefficient engine.

This is a real boundary. The coexistence argument is conditional: it holds if the dominant self-replicating system operates as life under the model's definition. Whether that condition is met is not something the model itself can guarantee. This is not a flaw in the model — it is an honest limit of what a descriptive physical framework can do.

### Open Questions

- Can factoring resistance be formalized mathematically? What does "scale" mean precisely — is it continuous or discrete? How do you enumerate scales without an observer choosing them?
- Are there fundamental physical limits to how much state diversity can be extracted from a given energy gradient?
- Does the model predict anything testable about where life should arise or what forms it should take?
- Can it be formally proven that the reachable state spaces of different physical substrates are non-overlapping, and if so, to what degree?
- Is there a selection pressure — physical, evolutionary, or otherwise — that favors diversity-compounding self-replicating systems over homogeneous ones? If so, does this make the emergence of "life" in the model's sense more likely than the emergence of non-diversifying replicators?
- Can the boundary between "life" (diversity-compounding replicators) and "non-life" (homogeneous replicators) be formalized, and does it predict observable differences in behavior or structure?
- Are there systems that resist factoring at every scale but would not qualify as life under this model? If so, what distinguishes them — and does that distinction reveal a gap in the definition?
- Does factoring resistance correspond to any known physical quantity, or is it a genuinely novel measure? If novel, what would be required to establish it formally?

---

### Appendix: Behavioral Observations (Not Part of the Core Model)

*This section is separated from the core model deliberately. The observations below are consistent with the model but are not evidence for it. Including them as part of the model's foundation would risk making it unfalsifiable — a framework that explains any behavior, including contradictory ones, explains nothing. This section is included as speculative commentary, not as structural support.*

**The pattern**

Human civilizations exhibit a broad trajectory from information-destroying behaviors toward information-preserving ones. Early history is marked by burned libraries, driven-extinct species, and lost languages. Over time, civilizations increasingly invest in the opposite: conservation of endangered species, archival of history, construction of museums, seed vaults, DNA databases, and digital preservation efforts. Humans generally do not frame these activities in information-theoretic terms. They are motivated by cultural values, aesthetic appreciation, scientific curiosity, or moral intuition — not by a conscious strategy of information maximization.

**Why this is not part of the core model**

The model describes a physical phenomenon — what life does at scale and over time. It does not claim that individual behaviors or cultural developments are driven by information maximization. Retrofitting the model onto specific human behaviors is tempting but methodologically unsound. Environmental destruction could just as easily be narrated as "the system clearing space for new information" or "the system not yet optimizing." If the model can explain both preservation and destruction after the fact, it has no predictive power and is functioning as a narrative rather than a framework.

Early humans were not unconsciously maximizing information. They were surviving under resource constraints with limited knowledge. Sometimes that produced information; sometimes it destroyed it. The model does not explain why any specific behavior occurred.

**What can be said carefully**

The disciplined version of this observation is predictive rather than retrospective. If the model is correct, it generates a testable expectation: information-preserving behaviors should increase over time in any sufficiently complex living system, because systems that maintain information diversity generate more total information than systems that don't, and selection pressures — cultural, evolutionary, or otherwise — should favor them over long timescales.

Human history is consistent with this prediction. That is a weaker claim than "the model explains human behavior," but it is a stronger claim epistemically, because it identifies something the model expects to see and that could in principle be wrong. A model that can be wrong is a model that means something.
