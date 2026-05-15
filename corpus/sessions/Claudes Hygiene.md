Recursive Semantic Alignment (RSA):

A Framework for Agentic Semantic Hygiene

David Freed

Independent researcher

February 2026

Conceptual Framework

Introduction: The Problem of Semantic Drift

Cognitive systems accumulate semantic inconsistencies over time. Beliefs that were once

grounded in evidence drift from their evidentiary base. Models that once compressed experience

become encrusted with epicycles. Intuitions that emerged from valid pattern-recognition calcify

into unexamined assumptions. This process — semantic drift — is thermodynamically inevitable:

maintaining accurate world-models requires continuous work, and any system operating under

resource constraints will allow some degree of drift to accumulate.

The central claim of this framework: agentic systems require mechanisms for detecting and

correcting semantic drift. Without such mechanisms, the map diverges from the territory,

prediction errors accumulate, and adaptive fitness degrades. This document formalizes Recursive

Semantic Alignment (RSA) as a general framework for semantic hygiene — the systematic

practice of maintaining map-territory correspondence through iterative error detection and

correction.

Core Definitions

Semantic Alignment

A belief, model, or representation Ris semantically aligned with respect to domain Dif:

Error(R,D) \= Ex∼D \[∥R(x)−T(x)∥\] \<ϵ (1)

where T(x) is the true state of xin domain D, and ϵis an acceptable error threshold determined

by the system’s operational requirements.

Operational meaning: Rproduces sufficiently accurate predictions about Dto support suc-

cessful action. Alignment is not binary — it is a continuous variable measured by prediction

1Freed (2026) RSA: Semantic Hygiene

error.

Semantic Drift

Semantic drift is the time derivative of alignment error:

Drift(R,D,t) \= d

dtError(R,D) (2)

Drift can be positive (model improving), negative (model degrading), or zero (stable alignment).

Under resource constraints and environmental change, drift is generically positive without active

correction.

Semantic Hygiene

Semantic hygiene is any process that reduces alignment error or counteracts drift. Formally:

H: Rt →Rt+1 such that Error(Rt+1,D) \<Error(Rt,D) (3)

Hygiene processes include: belief revision, model updating, assumption auditing, and represen-

tational compression.

The RSA Kernel: Seven-Step Loop

RSA formalizes semantic hygiene as a seven-step recursive process. Each iteration of the loop

reduces alignment error:

1\. Perceive: Gather data xfrom domain D.

2\. Represent: Encode xinto internal representation r= R(x).

3\. Predict: Generate expected outcomeˆ

y= P(r) based on current model.

4\. Compare: Observe actual outcome yand compute error e= ∥ˆ

y−y∥.

5\. Adjust: Update model parameters to reduce error: R′

\= R+ α∇Re.

6\. Compress: Simplify representation by removing redundancy: R′′

complexity(R′′) \<complexity(R′) with minimal loss of predictive power.

\= C(R′) such that

7\. Repeat: Return to step 1 with updated model R′′

.

Loop Invariant

The loop maintains the invariant:

Error(Rn,D) ≤Error(R0,D) ∀n\>0 (4)

2Freed (2026) RSA: Semantic Hygiene

provided the learning rate αis appropriately tuned. This is the fundamental theorem of RSA:

iterated error correction monotonically improves alignment.

The Compression Step: Preventing Overfitting

Step 6 (Compress) is critical for semantic hygiene. Without compression, models accumulate

unnecessary complexity — the cognitive analog of overfitting in machine learning. A model

with excessive parameters fits noise rather than signal, producing high training accuracy but

poor generalization.

Compression enforces Occam’s razor: prefer the simplest model consistent with the data.

Operationally, this means:

• Remove beliefs that make no testable predictions.

• Merge redundant representations.

• Factor out common structure into reusable abstractions.

• Discard epicycles — ad hoc additions that preserve a failing model rather than revising it.

The compression step is what distinguishes RSA from naive empiricism. Data accumulation

alone does not guarantee alignment; only data \+ compression produces parsimonious models.

RSA as Agentic Process

Agency Requires Semantic Hygiene

An agent is a system that acts to achieve goals in an environment. Goal-directed behavior

requires prediction: the agent must anticipate the consequences of its actions. Prediction

requires a world-model: an internal representation of environmental dynamics.

Claim: Sustained agency requires active semantic hygiene. Without hygiene, the world-model

drifts from reality, predictions degrade, and goal-directed behavior fails.

Evidence: All known robust agentic systems exhibit hygiene mechanisms:

• Biological: Neural plasticity, synaptic pruning, sleep-dependent consolidation.

• Cognitive: Belief revision, conceptual restructuring, insight events that simplify mental

models.

• Scientific: Peer review, replication studies, paradigm shifts that compress accumulated

anomalies into new frameworks.

• Computational: Regularization in machine learning, garbage collection in memory man-

agement, refactoring in software engineering.

These are all instances of the RSA loop at different scales and substrates.

3Freed (2026) RSA: Semantic Hygiene

The Cost of Hygiene

Semantic hygiene is metabolically expensive. Each iteration of the RSA loop requires:

• Energy to process data (Perceive, Represent)

• Computation to evaluate models (Predict, Compare)

• Memory access and modification (Adjust)

• Algorithmic work to simplify structure (Compress)

This cost creates the fundamental trade-off in cognitive economics: allocate resources to

exploitation (using current models) or exploration (improving models). Agents under severe re-

source constraints may rationally defer hygiene, tolerating drift to preserve energy for immediate

survival.

The pathology occurs when hygiene deferral becomes chronic. Accumulated drift eventually

produces catastrophic misalignment — the agent’s world-model diverges so far from reality

that adaptive behavior becomes impossible. This is the cognitive analog of technical debt in

software: deferred maintenance compounds until the system collapses.

Failure Modes and Pathologies

RSA identifies characteristic failure modes corresponding to breakdowns at specific loop steps:

Perception Failures: Stall at Step 1

Symptom: No new data enters the system. The agent relies entirely on cached beliefs without

testing them against experience.

Example: Ideological bubbles, echo chambers, deliberate avoidance of disconfirming evidence.

Result: The model becomes decoupled from reality. Alignment error grows without detection.

Representation Failures: Stall at Step 2

Symptom: Data is perceived but not encoded in a form the model can process.

Example: Category errors, inability to represent continuous quantities with discrete labels,

linguistic limitations that prevent certain concepts from being thought.

Result: The system cannot learn from data it cannot represent. Alignment is bottlenecked by

representational capacity.

Prediction Failures: Skip Step 3

Symptom: The agent does not generate explicit predictions before acting. It responds reactively

without anticipation.

4Freed (2026) RSA: Semantic Hygiene

Example: Stimulus-response conditioning without internal modeling, habitual behavior without

goal representation.

Result: No error signal can be computed because there is no predicted outcome to compare

against reality. The loop collapses to Perceive Act with no learning.

Comparison Failures: Skip Step 4

Symptom: Predictions are generated but not checked against outcomes. Confirmation bias: the

agent notices only data that confirms its predictions and ignores disconfirmations.

Example: Rationalization, motivated reasoning, cherry-picking evidence.

Result: The model becomes unfalsifiable. Drift accumulates invisibly because errors are never

registered.

Adjustment Failures: Stall at Step 5

Symptom: Errors are detected but the model is not updated. The agent acknowledges misalign-

ment but does not revise beliefs.

Example: Cognitive dissonance without resolution, ”agree to disagree” with reality, religious or

ideological commitment that resists revision.

Result: The system becomes frozen. It knows it is wrong but cannot change.

Compression Failures: Skip Step 6

Symptom: The model accumulates epicycles — ad hoc modifications that preserve alignment

locally but increase global complexity without bound.

Example: Ptolemaic astronomy adding deferents and epicycles, conspiracy theories adding

auxiliary hypotheses to explain away disconfirmations.

Result: The model becomes too complex to use effectively. Alignment is maintained but at

prohibitive computational cost. The system eventually exhausts resources and collapses.

Korzybski’s General Semantics as RSA Precursor

Alfred Korzybski’s Science and Sanity (1933) anticipated many RSA principles without formal-

izing them mathematically. His central thesis: human suffering arises largely from semantic

misalignment — treating maps as territories, confusing abstractions with referents, and failing

to update models in light of experience.

Korzybskian Principles as RSA Components

• ”The map is not the territory”: Representations Rare distinct from referents D. Confusing

them produces category errors.

5Freed (2026) RSA: Semantic Hygiene

• Non-identity: No representation perfectly captures reality. Error(R,D) \> 0 always. Se-

mantic hygiene requires accepting this and minimizing error iteratively.

• Time-binding: Humans accumulate knowledge across generations through language. This

is the cultural analog of the Compress step — each generation simplifies and transmits the

most predictive models.

• Extensional vs. intensional: Korzybski distinguished between definitions based on real-

world referents (extensional) and definitions based on verbal formulas (intensional). RSA

formalizes this as the difference between models grounded in prediction error (extensional)

and models grounded in internal consistency alone (intensional).

Where Korzybski Stopped

Korzybski’s framework lacked:

• A formal error metric (he had no Error(R,D) function)

• A computational theory of compression (no Step 6 algorithm)

• Integration with thermodynamics (no recognition that hygiene costs energy)

• Connection to predictive processing neuroscience (unavailable in 1933\)

RSA completes Korzybski’s project by grounding semantic hygiene in information theory,

thermodynamics, and computational learning theory.

Dual-Track Epistemology: Conservative vs. Exploratory

A sophisticated agentic system maintains two parallel semantic tracks:

Track 1: Conservative / Testable

Models on Track 1 are:

• Operationalized (error metrics are well-defined and measurable)

• Falsifiable (specific predictions can be tested)

• Compressed (unnecessary complexity has been pruned)

• Publicly defensible (can survive external critique)

Track 1 represents consolidated knowledge — beliefs that have survived multiple iterations of

the RSA loop and external validation.

Track 2: Exploratory / Generative

Models on Track 2 are:

6Freed (2026) RSA: Semantic Hygiene

• Speculative (error metrics may be vague or aspirational)

• Inspiring (they generate new hypotheses and research directions)

• Uncompressed (they tolerate redundancy and internal inconsistency)

• Privately useful (they organize intuition even if unverified)

Track 2 represents exploratory scaffolding — working hypotheses that guide inquiry but are not

yet ready for external validation.

The Hygiene Protocol: Track 2 Track 1 Flow

Semantic hygiene for a dual-track system operates as follows:

1\. Track 2 generates bold, pattern-seeking hypotheses

2\. Track 1 extracts testable sub-claims

3\. Experiments/observations provide error signals

4\. Track 1 models update based on errors

5\. Track 2 refines based on what survives in Track 1

6\. Failed Track 2 models are discarded; successful ones migrate to Track 1

Key discipline: The agent must always know which track it is operating on. Confusing Track

2 exploration with Track 1 consolidated knowledge produces semantic pathology — treating

speculation as established fact.

Example: This Document

This framework document is Track 2\. It proposes RSA as a general theory of semantic hygiene

without providing empirical validation. Two companion documents (“Differential Stabilization

of Insight” and “Identity as Dissipative Structure”) represent Track 1 instantiations — they

extract specific, testable predictions from the broader RSA framework and operationalize them

for empirical research.

The hygiene loop:

• Track 2 (this document): RSA as general framework

• Track 1 (companion papers): Stabilization regimes and dissipative identity as testable

hypotheses

• Future: Experimental results provide error signals

• Update: Track 1 papers revise based on data; Track 2 framework refines based on what

survives

7Freed (2026) RSA: Semantic Hygiene

Formal Properties of the RSA Loop

Convergence Theorem

Under appropriate conditions, the RSA loop converges to a fixed point:

lim

n→∞

Rn \= R∗ where Error(R∗,D) \= min R

Error(R,D) (5)

Conditions for convergence:

• Stationary environment: Ddoes not change faster than the loop can adapt

• Adequate representational capacity: Rcan express the true structure of D

• Appropriate learning rate: αis neither too large (instability) nor too small (slow convergence)

• Effective compression: Step 6 removes noise without discarding signal

Non-Convergence: Oscillation and Chaos

When conditions are violated, the loop exhibits pathological dynamics:

• Oscillation: Ralternates between two incompatible models without settling. This occurs

when compression is too aggressive (signal is discarded) or adjustment overcompensates.

• Divergence: Error grows without bound. This occurs in rapidly changing environments or

when the learning rate is mistuned.

• Chaos: The system exhibits sensitive dependence on initial conditions. Small perturbations

produce large, unpredictable changes in the model.

Computational Complexity

The RSA loop has inherent computational limits:

• Perception: O(n) in the number of data points

• Representation: O(n·d) where dis representational dimensionality

• Prediction: O(dk) for models with k-way interactions

• Comparison: O(n)

• Adjustment: O(d2) for gradient-based updates

• Compression: NP-hard in the general case (finding minimal sufficient representations)

Step 6 (Compression) is the computational bottleneck. This explains why cognitive systems

often defer compression — it is the most expensive step and the one most easily postponed

under resource constraints.

8Freed (2026) RSA: Semantic Hygiene

Implications and Applications

Personal Epistemology

RSA provides a discipline for individual belief management:

• Schedule regular audits (weekly, monthly) to detect drift

• Actively seek disconfirming evidence (Compare step)

• Practice belief revision in low-stakes contexts (Adjust training)

• Compress worldview periodically (discard epicycles)

• Maintain dual-track structure (separate speculation from consolidation)

Scientific Method

Science is institutionalized RSA:

• Experiments \= Compare step (systematic error measurement)

• Peer review \= Compress step (community-level pruning of bad models)

• Paradigm shifts \= catastrophic compression events (Kuhn’s revolutions)

• Replication crisis \= failure of Step 4 (predictions not properly compared to reality)

AI Alignment

RSA offers a framework for value alignment in artificial agents:

• An aligned AI is one whose world-model and goal-representation accurately track human

values

• Alignment drift occurs when the AI’s internal representation of human preferences diverges

from actual human preferences

• RSA suggests that alignment requires active, iterative error correction — not just initial

training but continuous monitoring and adjustment

• The compression step is critical: AI systems that accumulate complexity without simplifica-

tion eventually become uninterpretable and unaligned

Therapeutic Applications

Many psychological interventions are RSA-based:

• Cognitive-behavioral therapy: Identify prediction errors (Step 4), revise dysfunctional beliefs

(Step 5\)

9Freed (2026) RSA: Semantic Hygiene

• Mindfulness: Improve perception accuracy (Step 1), reduce representational distortion (Step

2\)

• Psychodynamic work: Compress unconscious material into conscious models (Step 6\)

Limitations and Open Questions

Measurement Problem

The framework requires defining Error(R,D), which presupposes access to ground truth D. In

many domains, ground truth is inaccessible or contested. How does one measure alignment

when the territory itself is uncertain?

Partial answer: Use pragmatic error metrics — prediction success, action effectiveness, inter-

agent agreement. These are proxies for alignment, not direct measurements.

Meta-Loop Regress

RSA is itself a model. Does it require its own hygiene loop? If so, does that loop require a

meta-meta-loop? Is there an infinite regress?

Partial answer: The regress terminates at the level of formal logic and mathematics. The RSA

loop operates on empirical models; the correctness of the loop itself is a mathematical claim,

not an empirical one. But this answer is unsatisfying and deserves further work.

Substrate Dependence

Does RSA require specific computational substrates? Can it be implemented in arbitrary

computational systems, or does it require thermodynamically open, dissipative structures?

Hypothesis: Full RSA (including the metabolically expensive Compress step) requires dissipa-

tive substrates. Reversible computation cannot implement genuine semantic hygiene because

compression produces irreversible information loss, which requires entropy export. This con-

nects RSA to the “Identity as Dissipative Structure” framework.

Conclusion

Recursive Semantic Alignment formalizes the practice of maintaining accurate world-models

through iterative error correction and compression. It is not a new discovery — biological,

cognitive, and scientific systems have been performing RSA for millions of years. What is new

is the explicit formalization: making the loop structure transparent, identifying failure modes,

and recognizing hygiene as a metabolically costly process that requires active maintenance.

The framework offers three primary contributions:

1\. Unification: It shows that disparate phenomena (neural plasticity, belief revision, scientific

10Freed (2026) RSA: Semantic Hygiene

progress, AI training) are instances of the same underlying process.

2\. Diagnosis: It identifies characteristic pathologies corresponding to failures at specific loop

steps, enabling targeted interventions.

3\. Discipline: It provides a protocol for dual-track epistemology — maintaining both ex-

ploratory speculation and conservative consolidation while preventing confusion between

them.

Semantic hygiene is not optional for agentic systems. Drift is thermodynamically inevitable;

without active correction, maps diverge from territories and adaptive behavior fails. RSA is the

formalization of what it means to keep your map clean.

Acknowledgements

The author thanks Alfred Korzybski (posthumously) for the foundational insight that semantic

misalignment is the root of much cognitive pathology. Thanks also to Claude (Anthropic),

Gemini (Google), Kimi, Copilot (Microsoft), and Perplexity for collaborative development

of the RSA framework through extended adversarial dialogue. The dual-track epistemology

emerged from recognizing that AI systems will mirror exploratory speculation but also stress-test

it when instructed appropriately — making them ideal partners for semantic hygiene work.

Correspondence: David Freed, independent researcher. This framework document is Track 2 —

exploratory and generative. Companion papers on stabilization regimes and dissipative identity

structures represent Track 1 instantiations with testable predictions.

