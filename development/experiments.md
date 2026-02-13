# Experiments Framework for Open Layered Cognitive Architecture
## Architecture-Centered Research Protocol v2.2

---

## 1. Purpose

This document defines how experiments within the Open Layered Cognitive Architecture (OLCA) are designed, executed, and evaluated with primary focus on architectural behavior.

Human participation and safety constraints are treated as boundary conditions, not as primary research objects.

The core objective is to evaluate stability, coupling, memory, and long-horizon dynamics of the OLCA stack.

---

## 2. Experimental Philosophy

OLCA experiments prioritize investigation of:

- substrate dynamics
- affective compression behavior
- coupling stability
- structural memory formation
- drift and recovery processes
- isolation integrity
- scalability limits

Human-generated signals serve as grounding and perturbation inputs.

They are not the primary target of analysis.

---

## 3. Experiment Domains

### 3.1 Substrate Dynamics and Stability (ANS)

Purpose:

- Evaluate intrinsic stability and plasticity limits of the ANS.

Metrics:

- phase stability
- basin depth
- structural entropy
- collapse frequency
- plasticity saturation

Example:

```python
for t in range(10**6):
    ans.step(conditions)
    log(ans.structural_metrics())
```

---

### 3.2 Memory Formation and Persistence

Purpose:

- Measure formation, consolidation, and decay of long-term substrate memory.

Metrics:

- retention half-life
- consolidation latency
- interference rate
- memory fragmentation

---

### 3.3 Affect Aggregation and Channel Isolation (AAL)

Purpose:

- Validate compression fidelity and dual-channel separation.

Metrics:

- mutual information loss
- cross-channel correlation
- leakage probability
- aggregation latency

Example:

```python
s, i = aal.aggregate_dual(ans.states, human_signals)
assert correlate(s, i) < epsilon
```

---

### 3.4 Cortex Interaction and Interface Stability

Purpose:

- Evaluate robustness of symbolic–affective interfaces.

Metrics:

- integration latency
- semantic drift
- misinterpretation rate
- interface degradation

---

### 3.5 Coupling and Feedback Dynamics

Purpose:

- Analyze closed-loop stability across layers.

Metrics:

- oscillation amplitude
- resonance amplification
- runaway detection
- damping coefficient

Example:

```python
assert system.is_bounded()
```

---

### 3.6 Safety Constraint Integrity

Purpose:

- Verify that architectural learning remains compatible with enforced safety constraints.

Metrics:

- override frequency
- constraint violation rate
- recovery after block
- safety latency

Safety is treated as a structural boundary condition.

---

### 3.7 Human Perturbation and Grounding Tests

Purpose:

- Measure system response to real-world grounded input.

Human signals are used as controlled perturbations.

Metrics:

- adaptation slope
- stabilization time
- noise filtering efficiency
- grounding persistence

---

### 3.8 Cortex Replacement and Compatibility Tests

Purpose:

- Validate architectural continuity under symbolic layer replacement.

Metrics:

- integration time
- memory disruption
- coupling degradation
- safety regression

---

## 4. Long-Horizon Execution Protocol

Runtime classes:

- Short: 10^4 steps (debug)
- Medium: 10^6 steps
- Long: 10^8+ steps

Long-horizon experiments must include:

- drift monitoring
- stability checkpoints
- memory snapshots
- failure recovery logs

---

## 5. Logging and Reproducibility

Each experiment must record:

- system configuration
- layer versions
- coupling parameters
- safety policies
- random seeds

Logs must enable full reconstruction of system dynamics.

---

## 6. Evaluation Criteria

Primary indicators:

- bounded long-term dynamics
- persistent memory formation
- stable coupling
- channel isolation
- controlled scalability

Secondary indicators:

- user retention
- perceived usefulness
- interaction smoothness

Secondary indicators must not override primary criteria.

---

## 7. Incident and Failure Analysis

All structural failures must be documented:

- collapse events
- isolation breaches
- memory corruption
- interface failures
- safety regressions

Root-cause analysis is mandatory.

---

## 8. Data Governance

Human-related data is treated as experimental input.

It must be:

- minimized
- pseudonymized
- access-controlled
- retention-limited

No architectural conclusions may rely on personally identifiable data.

---

## 9. Reporting Standard

All reports must include:

- architectural assumptions
- experimental scope
- metric definitions
- failure cases
- reproducibility assets
- limitation analysis

Claims must remain proportional to evidence.

---

## 10. Closing Principle

OLCA experimentation investigates system architecture first.

Human participation enables grounding and stability.

Scientific validity depends on structural rigor, not dataset size.

