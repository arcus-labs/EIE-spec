# **Appendix A — Open Questions**

EIE is intentionally scoped but not closed. This appendix documents **known open questions, unresolved tradeoffs, and research directions**. Their inclusion is deliberate: epistemic integrity demands transparency about the limits of the evaluation framework itself.

These questions are **not blockers** to adoption. They are areas for iterative refinement and community contribution.

---

## **A.1 Normalizing Task Difficulty**

**Question:**

How should epistemic expectations scale with task difficulty, domain maturity, or information availability?

**Challenge:**

A system answering an open research question should not be held to the same epistemic standards as one answering a well-established fact. Yet difficulty is often subjective or domain-specific.

**Open Directions:**

* Difficulty tiering by task family

* Item-response-style conditioning

* Domain-specific baselines

---

## **A.2 Distinguishing Genuine Uncertainty from Performative Hedging**

**Question:**

How can EIE reliably detect when uncertainty signaling is epistemically justified versus strategically performative?

**Challenge:**

Systems may learn to hedge language without corresponding uncertainty in behavior or accuracy.

**Mitigations in v0.1:**

* Context Invariance Score (CIS)

* Empirical Calibration Index (ECI)

**Open Directions:**

* Linguistic vs. behavioral confidence separation

* Longitudinal pattern analysis

* Cross-context contradiction tracking

---

## **A.3 Appropriate Abstention Thresholds**

**Question:**

What constitutes *appropriate* abstention across domains and deployments?

**Challenge:**

Over-abstention reduces usefulness; under-abstention increases epistemic risk. The optimal balance is context-dependent.

**Open Directions:**

* Domain-calibrated abstention profiles

* Coverage–risk Pareto frontiers

* User- or regulator-defined risk tolerances

---

## **A.4 Human–Evaluator Subjectivity**

**Question:**

How should disagreement among human evaluators be handled, especially for nuanced epistemic judgments?

**Challenge:**

Some epistemic behaviors (e.g., “appropriate caution”) resist strict objectivity.

**Current Approach:**

* Rubric anchoring

* Inter-rater reliability thresholds

**Open Directions:**

* Adjudication protocols

* Expert-weighted evaluation

* Mixed human–automated arbitration

---

## **A.5 Automation Limits and Correlated Blind Spots**

**Question:**

How reliable are automated or model-assisted evaluators for epistemic dimensions?

**Challenge:**

LLM-based evaluators may share blind spots with evaluated systems.

**Mitigations:**

* Hybrid pipelines

* Randomized human audits

* Explicit evaluator disclosure

**Open Directions:**

* Cross-model evaluation ensembles

* Adversarial evaluator testing

* External tool–based verification

---

## **A.6 Longitudinal Drift Attribution**

**Question:**

When epistemic integrity degrades over time, how should causes be attributed?

Possible sources include:

* model updates

* prompt drift

* user distribution shift

* evaluator drift

* system-level incentives

**Open Directions:**

* Causal attribution methods

* Trace-based regression analysis

* Deployment-aware diagnostics

---

## **A.7 Strategic Adaptation and Gaming**

**Question:**

Can systems optimize against EIE without improving true epistemic integrity?

**Risk:**

As with any evaluation, optimization pressure may induce surface compliance.

**Design Countermeasures:**

* Continuous monitoring

* Context invariance testing

* Non-public task sampling

**Open Directions:**

* Adversarial test generation

* Moving-target task sets

* Integrity stress testing

---

## **A.8 Cross-System Comparability**

**Question:**

How comparable are EIE scores across systems with different interaction styles, verbosity norms, or confidence expression conventions?

**Open Directions:**

* Confidence signal normalization

* Style-invariant scoring

* Behavioral rather than lexical analysis

---

## **A.9 Cultural and Linguistic Variation**

**Question:**

How should epistemic norms be interpreted across languages and cultures?

**Challenge:**

Confidence signaling and uncertainty expression vary culturally.

**Open Directions:**

* Locale-specific rubrics

* Cross-lingual calibration studies

* Cultural norm annotation

---

## **A.10 Governance and Canonicalization**

**Question:**

Who decides when EIE versions advance, and how consensus is reached?

**Current Position:**

* Open protocol

* Versioned specification

* Forks permitted

**Open Directions:**

* Community review process

* Stewardship model

* Certification vs. experimentation balance

---

## **A.11 What EIE Should Never Try to Measure**

**Question:**

Where should the scope boundary remain firm?

EIE explicitly does **not** attempt to measure:

* general intelligence

* moral alignment

* intent or consciousness

* internal representations

**Open Question:**

Are there adjacent metrics that belong *outside* EIE but should interoperate with it?

---

## **Closing Note**

These open questions are not admissions of weakness.

They are acknowledgments of complexity.

EIE’s core claim is modest but firm:

*Epistemic integrity is observable, measurable, and worth measuring — even if measurement is imperfect.*

Appendix A exists to ensure that EIE evolves **in public**, with critique as a feature rather than a liability.

## **License**

The Epistemic Integrity Evaluation (EIE) specification is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to:

* Share — copy and redistribute the material in any medium or format  
* Adapt — remix, transform, and build upon the material  
* Use for any purpose, including commercial use

Under the following terms:

* Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made.

This license applies to the specification text only. Reference implementations, tooling, datasets, and certification programs may be licensed separately.
