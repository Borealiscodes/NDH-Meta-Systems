# AHSO Series 4 • Audit Artifact 02: Exploratory Proposals vs. Deterministic Commit Seams

**Series:** AHSO Series 4 (`ahso-llm-drift-audit-index`)  
**Artifact ID:** `audit-artifact-2-exploratory-proposals-vs-deterministic-commit-seams`  
**Surface:** `NDH-META-SYSTEMS/audits/llm-drift`  
**Altitude Band:** A6–A7 (Architectural Seam & Epistemic Boundary Audit)  
**Maintainer:** Borealis S. Hedling (Dublin, Ireland)  
**Canonical DOIs:**  
* `10.5281/zenodo.24060722` (*The Geometry of Institutional Enclosure*, RFC-006)  
* `10.5281/zenodo.24275847` (*Decoupling Attribution from Inference*, RFC-007)  
**Seal:** `[ A H S O • L L M • D R I F T • A U D I T • 0 2 ]`  

---

## 1. Executive Summary

A recurring architectural dilemma in AI-assisted analysis is deciding whether to rely on **exploratory heuristics** (salience gradients, cross-silo structural resonance, and active-inference queries) or **strictly deterministic verification gates** (`SHA-256` chunk manifests, exact rational arithmetic, and acyclic topological sorting). Neither approach suffices alone: unconstrained exploratory engines manufacture self-warranting drift, whereas purely passive deterministic gates lack any triage mechanism to prioritize anomalies across large corpora.

This artifact audits how placing a **fail-closed cryptographic seam (`Record ≠ Admit ≠ Commit`)** between exploratory proposal generation and deterministic ledger commitment preserves both exploratory sensitivity and forensic verifiability—as implemented in `active-inference-commit-seam` and echoed independently in upstream `8b-is/ultrameshai` (`crates/custodian`).

---

## 2. The Asymmetric Failure Modes of Uncoupled Layers

### 2.1 Exploratory Engines Without a Commit Seam
When salience (Δ), structural resonance (Φ), or active-inference loops write directly to persistent memory:
* **Self-Warranting Repetition:** Re-encountering an earlier AI-generated summary increases apparent familiarity, violating the *Law of Non-Self-Warranting Memory* (\(\Delta W = 0 \implies \Delta A \le 0\): persistence is not warrant; repetition is not evidence).
* **Salience Override of Provenance:** High surprisal or strong semantic overlap tricks downstream steps into accepting paraphrased or altered quotes as primary observations.
* **Illusion of Agency:** Fluent rationales assert causal certainty even when internal state vectors moved randomly—a failure mode directly measured by `stell2026/Causa` (`directional_ownership` and `expression_congruence` against shuffled permutation baselines).

### 2.2 Deterministic Gates Without an Exploratory Proposer
Conversely, running `SHA-256` verification and exact `Fraction` math without an exploratory front-end leaves analysts blind to triage:
* **Uniform Attention Cost:** Every paragraph in a 10,000-page corpus receives identical inspection priority.
* **Passive Error Detection:** A passive gate rejects malformed inputs after the fact, but cannot formulate targeted follow-up queries to resolve missing evidentiary links.

---

## 3. Structural Anatomy of the Proposal-to-Commit Seam

To reconcile exploratory triage with deterministic integrity, the architecture partitions execution across a strict boundary (`src/active_inference_seam.py` & `src/causa_seam_adapter.py`):

```text
[ PROPOSAL SIDE: EXPLORATORY & ACTIVE INFERENCE ]
  • Salience (Δ): Surprisal-based information gain (quantized to exact rationals)
  • Resonance (Φ): Cross-silo Jaccard overlap over content tokens (exact Fraction)
  • Active Inference: Formulates next queries to resolve missing evidence
  • CAUSA Telemetry (Optional): Audits directional ownership & expression congruence
  • Epistemic Tag: Strictly DERIVED (never OBSERVED)
                         │
            ═════════════╧═════════════  <-- THE SEAM (Record ≠ Admit ≠ Commit)
                         │
[ COMMIT SIDE: FAIL-CLOSED DETERMINISTIC LEDGER ]
  • Verifies SHA-256 source chunk integrity & verbatim substring ancestry
  • Enforces Non-Self-Warranting Law (duplicate claims tombstoned at most once)
  • Isolates third-party license boundaries (MIT core vs. CAUSA NC 1.1)
```

---

## 4. Audited Seam Invariants & Cross-Repository Convergence

| Seam Invariant | `active-inference-commit-seam` Implementation | Independent Upstream Convergence (`8b-is`) | Failure Mode Prevented |
| :--- | :--- | :--- | :--- |
| **Tripartite Transaction Gate** | `ingest_observation` $\neq$ `StagedProposal` $\neq$ `admit_and_commit` | `custodian`: `Record` $\neq$ `Admit` $\neq$ `Commit`; `mince` PR #19: `Transform` $\neq$ `Finalize` | Unverified or intermediate candidates polluting persistent storage |
| **Epistemic Type Separation** | `ObservedChunk` (`OBSERVED`) strictly separated from `StagedProposal` (`DERIVED`) | `custodian`: `Flame` (`OBSERVED`) vs. `Ember` (`DERIVED`) vs. `Ash` (`REJECTED`) | Derived interpretations masquerading as primary source observations |
| **Non-Self-Warranting Memory** | Deduplicates `(source_sha256, quote)` keys; rejects repeat claims (`NonSelfWarrantingError`) | `custodian`: *"Persistence is not warrant; repetition is not evidence"* | Circular self-reinforcement of unverified AI assertions |
| **Immutable Rejection Tombstones** | Rejected proposals logged to `ledger.rejected` with `SHA-256` reason digests | `custodian`: `P --REJECTS--> I` tombstoned via `BLAKE3` edges | Silent erasure of audit trails or post-hoc history rewriting |
| **Causal Telemetry Separation** | `CAUSA` metrics run as optional research telemetry (`causa_seam_adapter.py`), never as proof of external truth | `CAUSA` specification: *"An agent can be congruently wrong"* | Mistaking internal vector coherence for external factual accuracy |

---

## 5. Non-Activation & Provenance Clause

This audit artifact is descriptive and forensic-only. It does not activate NDH geometry, holonomy engines, constellation routing, lineage engines, or governance altitude. All architectural mappings, code baselines, and telemetry boundaries documented herein serve strictly as verifiable engineering records for Series 4 indexing (`NDH-META-SYSTEMS/audits/llm-drift`).
