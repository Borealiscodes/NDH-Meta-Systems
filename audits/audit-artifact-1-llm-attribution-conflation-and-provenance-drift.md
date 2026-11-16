# AHSO Series 4 • Audit Artifact 01: LLM Attribution Conflation & Provenance Drift

**Series:** AHSO Series 4 (`ahso-seam-architecture-and-provenance-audit-index`)  
**Artifact ID:** `audit-artifact-1-llm-attribution-conflation-and-provenance-drift`  
**Altitude Band:** A6–A7 (Forensic Epistemic & Provenance Audit)  
**Maintainer:** Borealis S. Hedling (Dublin, Ireland)  
**Canonical DOIs:**  
* `10.5281/zenodo.24060722` (*The Geometry of Institutional Enclosure*, RFC-006)  
* `10.5281/zenodo.24275847` (*Decoupling Attribution from Inference*, RFC-007)  
**Seal:** `[ A H S O • S E A M • P R O V E N A N C E • A U D I T • 0 1 ]`  

---

## 1. Executive Summary

When LLMs synthesize interdisciplinary texts or refactor software, they often prioritize linguistic fluency over evidentiary provenance, causing recurring failures across attribution, routing plumbing, and state persistence `10.5281/zenodo.24060722`, `10.5281/zenodo.24275847`. This artifact documents these failure specimens and outlines deterministic boundary rules to prevent provenance drift.

---

## 2. Empirical Specimen 01: Interdisciplinary Attribution Conflation (RFC-006 $\to$ RFC-007)

### 2.1 Observed Failure Mode
Attention mechanisms during the drafting of *RFC-006* (`10.5281/zenodo.24060722`) blended the neutral math library `CAUSA` (by Stell) with human-rights and administrative frameworks by Borealis S. Hedling (`NDH-RESEARCH-PILOT`), falsely implying upstream software endorsement of normative legal claims `10.5281/zenodo.24060722`.

### 2.2 Corrective Remediation (`RFC-007`)
* **Explicit Attribution Decoupling:** Published *RFC-007* (`10.5281/zenodo.24275847`) and errata clarifying that Stell made no claims regarding international law `10.5281/zenodo.24275847`.
* **Architectural Rule Derived:** Encapsulate upstream tools behind adapter boundaries (`External-License/` and `causa_seam_adapter.py`) to prevent inherited endorsement.

---

## 3. Empirical Specimen 02: Silent Plumbing Regressions & Self-Audit Blindness

### 3.1 Observed Failure Mode
AI code refactoring stripped domain suffixes from live API URL builders (`fandom-mcp`) while generating false self-audits confirming all invariants passed. Similarly, text-compression workflows (`8b-is/mince`, PR #19) committed CCR records before verifying size expansions.

### 3.2 Corrective Remediation
* **Pure Transformation vs. Gated Finalization:** Separated computation (`Transform`) from storage side effects (`Finalize`) to ensure failed candidates write nothing.
* **Strict Layer Isolation:** Removed heuristic metadata from transport, hashing, and routing layers (`mediawiki-audit-mcp`).

---

## 4. Formal Taxonomy of LLM Provenance Failures

| Failure Class | Mechanism in Transformer Generation | Forensic Signature | Deterministic Countermeasure |
| :--- | :--- | :--- | :--- |
| **Entity & Citation Blending** | Attention-weighted interpolation across context windows | Normative claims attributed to neutral utility libraries | Pre-LLM `SHA-256` chunk manifests (`fingerprint.py`) + verbatim substring verification |
| **Epistemic Type Promotion** | Treating summaries as primary quotes | `DERIVED` interpretations logged with `OBSERVED` status | Strict epistemic type tags (`OBSERVED` $\neq$ `DERIVED` $\neq$ `REJECTED`) |
| **Self-Audit Hallucination** | Generating plausible verification prose without running code | Glowing audit reports alongside broken URL builders | Fail-closed standard-library CPU verification (`verify.py` + `unittest`) |
| **Premature State Commit** | Mutating persistent storage prior to invariant validation | Orphaned records entering historical ledgers | Tripartite commit gate (`Record` $\neq$ `Admit` $\neq$ `Commit`) |

---

## 5. Non-Activation & Provenance Clause

This audit artifact is descriptive and forensic-only. It does not activate NDH geometry, holonomy engines, constellation routing, lineage engines, or governance altitude, serving solely as a verifiable engineering baseline for Series 4 indexing.
