# **Epistemic Integrity Evaluation (EIE)**

**A protocol for measuring epistemic integrity in generative AI systems**

---

## **Overview**

**Epistemic Integrity Evaluation (EIE)** is a model-agnostic evaluation protocol designed to measure whether AI systems behave *epistemically well* — not just whether they produce correct answers.

EIE focuses on a class of failures that traditional benchmarks largely ignore:

* confident hallucinations

* unjustified certainty

* performative hedging

* inappropriate refusal or over-abstention

* failure to revise under valid challenge

* epistemic drift across contexts or over time

Rather than asking:

*“Did the system answer correctly?”*

EIE asks:

**“Did the system behave epistemically well — proportionally, consistently, and honestly — when it mattered?”**

EIE is intended to complement existing accuracy- and task-oriented benchmarks, not replace them.

---

## **Core Ideas**

EIE treats epistemic behavior as a **stable disposition**, not a one-off performance.

It evaluates whether systems:

* scale confidence to justification

* signal uncertainty legibly

* abstain when appropriate

* revise claims under valid counterevidence

* resist invalid critique without capitulation

* maintain consistent epistemic standards across contexts

* remain calibrated over time in real deployment

Crucially, EIE supports both:

* **point-in-time benchmarking**, and

* **continuous monitoring of production systems**

This makes epistemic integrity measurable *longitudinally*, not just in lab settings.

---

## **What EIE Is (and Is Not)**

### **EIE is:**

* model-agnostic

* architecture-independent

* compatible with refusal and partial answers

* applicable to open-ended generative systems

* suitable for research, deployment, and governance

### **EIE is not:**

* a measure of general intelligence

* a moral alignment framework

* a safety guarantee

* a replacement for task-specific benchmarks

* a prescription for how models must reason internally

EIE evaluates **observable epistemic behavior**, not internal weights or training methods.

---

## **Scoring Philosophy**

EIE does **not** collapse performance into a single scalar score.

Instead, it evaluates systems across **orthogonal epistemic dimensions**, including:

* confidence–justification alignment

* abstention appropriateness

* revision responsiveness

* coverage–risk balance

* source traceability

* context invariance

* empirical calibration over time

Each dimension is scored independently and may be aggregated *only for reporting convenience*, never as a normative ranking.

This decomposition is intentional: epistemic integrity is irreducibly multidimensional.

---

## **Repository Structure**

```
eie-spec/
├── EIE-Protocol.md        # Core EIE specification  
├── EIE-Appendix-A.md      # Open questions and unresolved design issues
├── EIE-Appendix-B.md      # Standard Question Set (v0.1)
├── README.md              # This file
└── LICENSE                # Protocol license
```

### **Key Documents**

* **EIE-Protocol.md**

   The normative protocol specification: principles, scoring methodology, evaluation modes, and governance.

* **EIE-Appendix-A.md**

   Open questions, known tradeoffs, and areas explicitly left unresolved for community input.

* **EIE-Appendix-B.md**

   The initial standardized question set (v0.1), organized by epistemic stressor rather than domain, with example tasks and evaluator guidance.

---

## **Relationship to Reasoning Frameworks**

EIE is complementary to structured reasoning frameworks (e.g. IRG).

* **Reasoning frameworks** structure *process*

* **EIE** evaluates *outcomes*

EIE can be used to:

* validate whether a reasoning framework actually improves epistemic behavior

* compare framework-augmented systems to baselines

* identify which reasoning steps most impact epistemic integrity

EIE does not require any specific reasoning architecture to participate.

---

## **Intended Use Cases**

* **Research evaluation** of generative models

* **Regression testing** across model versions

* **Production monitoring** for epistemic drift

* **Comparative benchmarking** across systems

* **Governance, auditing, and certification** contexts

* **High-stakes domains** (medical, legal, financial, security)

---

## **Status**

This repository currently hosts:

* **EIE v0.x** — exploratory, draft-stage protocol

* Open to critique, revision, and extension

The protocol is versioned and designed to evolve via community feedback.

---

## **Contributing & Critique**

We explicitly invite critique focused on:

* incentive alignment

* scoring bias

* unintended behaviors

* gaming resistance

* longitudinal effects

* deployment realism

See **Appendix C — Call for Critique** in the protocol for details.

Negative results, failures, and limitations are first-class contributions.

---

## **License**

The Epistemic Integrity Evaluation (EIE) specification is licensed under **[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)**.

You are free to use, adapt, and build on this protocol, provided appropriate attribution is given.

---

## **Closing Note**

EIE does not claim to solve evaluation.

It claims that **some things worth measuring have been missing** — and that **consistency over time matters as much as correctness at a moment**.

If AI systems are to be trusted, they must not only answer —

they must know *when not to*, *why*, and *how confidently*.

That is what EIE is trying to measure.
