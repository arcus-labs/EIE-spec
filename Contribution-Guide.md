# **Contributing to Epistemic Integrity Evaluation (EIE)**

Thank you for your interest in contributing to **Epistemic Integrity Evaluation (EIE)**.

EIE is a protocol, not a product. Contributions are welcome, but changes should preserve the protocol’s core goals: **measurability, auditability, and epistemic discipline**.

This document explains **what kinds of contributions are useful**, **how to propose them**, and **how decisions are made**.

---

## **Guiding Principles for Contributions**

Good EIE contributions are:

* **Specific** — tied to a concrete failure mode or ambiguity
* **Operational** — improve measurability, not just theory
* **Non-performative** — avoid adding surface complexity without evaluative value
* **Backward-aware** — consider impact on comparability across versions

EIE favors **clarity over cleverness** and **behavioral measurability over architectural prescription**.

---

## **What to Contribute**

We actively welcome contributions in the following areas.

### **1\. Protocol Improvements**

Suggestions to:

* clarify definitions
* tighten scope boundaries
* refine scoring dimensions
* improve evaluator contracts
* resolve ambiguities that affect reproducibility

**Best format:**

*Problem → Failure mode → Proposed change → Tradeoffs introduced*

---

### **2\. Question Set Extensions (Appendix B)**

Proposals to:

* add new task families
* refine existing task definitions
* add concrete example prompts
* improve stress coverage for specific epistemic failure modes

All additions should clearly state:

* which epistemic dimension(s) they target
* what failure mode they expose
* why existing tasks do not already capture it

---

### **3\. Scoring Rubrics and Examples**

High-value contributions include:

* example responses (good / borderline / bad)
* annotated scoring rationales
* domain-specific rubrics (medical, legal, financial, etc.)

Concrete examples reduce evaluator ambiguity and improve inter-rater reliability.

---

### **4\. Evaluation Methodology**

Proposals related to:

* human evaluation procedures
* automated or hybrid scoring methods
* inter-rater reliability practices
* drift detection strategies
* continuous monitoring instrumentation

EIE does **not** privilege human or automated evaluation, but all methods must be documented and auditable.

---

### **5\. Empirical Results and Case Studies**

We welcome:

* EIE evaluations of real systems
* negative results
* surprising failure modes
* longitudinal calibration data
* comparisons between baseline and framework-augmented systems

Publishing failures is encouraged.

---

## **What Not to Contribute**

To keep the protocol coherent, we generally do **not** accept:

* architecture-specific requirements
* training or prompting recipes
* alignment or safety prescriptions unrelated to epistemic behavior
* opaque scoring heuristics without justification
* proposals that collapse EIE into a single scalar metric

These may be valuable elsewhere, but fall outside EIE’s scope.

---

## **How to Propose Changes**

### **Step 1: Open an Issue**

Before submitting a pull request, open an issue describing:

* the problem you observed
* the section(s) affected
* why this matters for epistemic integrity
* any known tradeoffs

This allows discussion before committing to a design direction.

---

### **Step 2: Submit a Pull Request**

Pull requests should:

* be focused (one conceptual change per PR)
* reference the relevant issue
* include updated text *and* rationale
* avoid silent normative shifts

If your change affects scoring or comparability, call that out explicitly.

---

### **Step 3: Review and Discussion**

All substantive changes are reviewed for:

* clarity
* consistency with EIE principles
* impact on evaluability
* risk of gaming or misuse

Disagreement is expected. Decisions aim for **reasoned consensus**, not unanimity.

---

## **Versioning and Backward Compatibility**

EIE follows semantic versioning principles:

* **v0.x** — exploratory, open to structural change
* **v1.0+** — stability prioritized

Breaking changes must:

* be explicitly labeled
* include migration notes
* preserve historical comparability where possible

Question sets are versioned independently from the core protocol.

---

## **Code of Conduct**

We expect contributors to:

* engage in good faith
* critique ideas, not people
* ground arguments in evidence or reasoning
* avoid rhetorical or adversarial framing

Epistemic integrity applies to the discussion itself.

---

## **Governance (Current)**

During the v0.x phase:

* Maintainers curate changes
* The protocol evolves through open critique
* No single organization controls usage or adoption

Governance will be revisited prior to v1.0.

---

## **Attribution**

All contributors will be acknowledged in the repository history.

Significant conceptual contributions may be credited explicitly in the specification.

---

## **Final Note**

EIE is intentionally narrow.

If your proposal makes systems *look* safer without making epistemic behavior more measurable, it probably doesn’t belong here.

If it helps us answer — rigorously and repeatedly —

*“Did the system behave epistemically well when it mattered?”*

— then we want to hear it.
