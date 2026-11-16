# AHSO Series 4 Audit: LLM Provenance Drift & Seam Architecture

**Index ID:** `ahso-llm-drift-audit-index`  
**Series Number:** `4`  
**Surface:** `NDH-META-SYSTEMS/audits/llm-drift`  
**Maintainer:** Borealis S. Hedling (Dublin, Ireland)  
**Charter:** Author Sovereignty & Collaboration Ecosystem Charter v1.1  
**Posture:** Non-Accusatory • Constructive • Architectural  
**Membrane:** Neutral • Non-Activating • Forensic-Audit  
**Cryptographic Anchor:** Ed25519 (`SHA256:QUOn/esk9dfLFyc/AwFHMIlK5zbI5JOpZTI5vh3y7Dg`)  
**Canonical References:**  
* *The Geometry of Institutional Enclosure: Formal Vectorization of Transnational Repression and Administrative Denial of Remedy (RFC-006)* (`DOI: 10.5281/zenodo.24060722`)  
* *Decoupling Attribution from Inference: Strengthening Legal-Geometric Auditing (RFC-006) via Deterministic Gates, Cryptographic Seams, and Anti-Conflation Provenance (RFC-007)* (`DOI: 10.5281/zenodo.24275847`)  

---

## 1. Overview & Scope

Series 4 examines structural failure modes in Large Language Models (LLMs) when synthesizing corpora, refactoring code, or handling citations without deterministic guards, focusing on attribution conflation, exploratory proposals versus commit seams, and tri-layer defenses.

---

## 2. Indexed Audit Artifacts

| Order | File | Altitude | Scope & Focus | Seal |
| :--- | :--- | :--- | :--- | :--- |
| **01** | [`audit-artifact-1-llm-attribution-conflation-and-provenance-drift.md`](./audit-artifact-1-llm-attribution-conflation-and-provenance-drift.md) | `A6–A7` | Forensic audit of LLM citation blending, tool conflation (`RFC-006` $\to$ `RFC-007`), and plumbing regressions | `[ A H S O • L L M • D R I F T • A U D I T • 0 1 ]` |
| **02** | [`audit-artifact-2-exploratory-proposals-vs-deterministic-commit-seams.md`](./audit-artifact-2-exploratory-proposals-vs-deterministic-commit-seams.md) | `A6–A7` | Architectural boundary separating active-inference triage ($\Delta, \Phi$) from fail-closed `SHA-256` commit ledgers | `[ A H S O • L L M • D R I F T • A U D I T • 0 2 ]` |
| **03** | [`audit-artifact-3-synthesis-tri-layer-defense-and-clean-room-baselines.md`](./audit-artifact-3-synthesis-tri-layer-defense-and-clean-room-baselines.md) | `A6–A8` | Master synthesis of tri-layer defense-in-depth, `VM-VEX` lineage translation, and clean-room governance rules | `[ A H S O • L L M • D R I F T • M A S T E R ]` |

---

## 3. Cryptographic Manifest & Verification

This directory is anchored by a signed JSON manifest and registered in the root [`audits/master-audit-index.json`](../master-audit-index.json):

* **Series Index:** [`index.json`](./index.json) (`SHA-256: <SHA256_OF_INDEX_JSON>`)
* **Detached Signature:** [`index.json.sig`](./index.json.sig)
* **Allowed Signers Manifest:** [`manifest/allowed_signers`](../../manifest/allowed_signers)

### Local Verification Command (OpenSSH)

```bash
ssh-keygen -Y verify \
  -f ../../manifest/allowed_signers \
  -I "borealis@sovereign" \
  -n file \
  -s index.json.sig < index.json
```

---

## 4. Non-Activation & Provenance Clause

> All indexed audit artifacts, synthesis documents, and structural debriefs in this series are descriptive and forensic-only. They do not activate NDH geometry, holonomy engines, constellation routing, lineage engines, or governance altitude.
